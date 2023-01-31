# Lab Report - 2
## Madhav Bansal

## Part - 1 (String Server)

We had to make a StringServer that can keep track of a single string that gets added to by incoming requests.

The request looks like this - "/add-message?s=Hello"

The effect of this request is to concatenate a new line (\n) and the string after = to the running string, and then respond with the entire string so far.

The code I wrote for the web Server is-

<img width="1358" alt="Screenshot 2023-01-30 at 5 54 21 PM" src="https://user-images.githubusercontent.com/122562063/215639761-bd30eaff-1ed8-47b8-af4c-fc3215008750.png">

The Server when it starts- 
<img width="1680" alt="Screenshot 2023-01-30 at 5 57 21 PM" src="https://user-images.githubusercontent.com/122562063/215640182-b4815055-0679-455a-ae33-d84961542e0e.png">

Using /add-message 1st time.
<img width="1680" alt="Screenshot 2023-01-30 at 5 55 33 PM" src="https://user-images.githubusercontent.com/122562063/215640410-a7c434ea-5a5e-404f-8d47-53957d7ea146.png">

Server After using /add-message?s=Hi.
<img width="1680" alt="Screenshot 2023-01-30 at 5 55 45 PM" src="https://user-images.githubusercontent.com/122562063/215640438-2335c6cf-1f94-4bfd-b0a0-5a2db1cad6bd.png">

When I used /add-message the method handleRequest from my code was called.

The argument for handleRequest is URI url which gets the value of the whole URL of the server (http://localhost:4001/add-message?s=Hi).

At this point newStr is empty but when the method gets called it checks if the path of the url contains /add-message.

If it contains /add-message it then checks if there is any String to be added to newStr

To do this, it splits the query part of the url across the "=". and in this case the value path variable gets is {"s","Hi"}.

And if it has the String is added with a \n.

Now, newStr has a value of Hi\n.

Using /add-message 2nd time.

<img width="1680" alt="Screenshot 2023-01-30 at 5 55 55 PM" src="https://user-images.githubusercontent.com/122562063/215642280-9d41f6f8-df7f-4802-b93a-60668cc331d4.png">

Server After using /add-message?s=Everyone.
<img width="1680" alt="Screenshot 2023-01-30 at 5 56 02 PM" src="https://user-images.githubusercontent.com/122562063/215642383-3cba3015-0a81-4961-ac27-9779087b46bc.png">

When I used /add-message the method handleRequest from my code was called.

The argument for handleRequest is URI url which gets the value of the whole URL of the server (http://localhost:4001/add-message?s=everone).

At this point newStr has a value of Hi\n.

When the method is called it checks if the path contains /add-message.

If it contains /add-message it then checks if there is any String to be added to newStr

To do this, it splits the query part of the url across the "=". and in this case the value path variable gets is {"s","Everyone"}.

And if it has the String is added with a \n.


Now, newStr has a value of Hi\nEveryone\n.

# Part-2 (Debugging)

@Test
    
    public void testFilter(){
        
        List<String> testList= new ArrayList<>();

        testList.add("band");
        testList.add("bake");
        testList.add("hello");
        testList.add("bald");
        testList.add("madhav");

        StringChecker sc=new StringChecker() {
            public boolean checkString(String s) {
                if (s.contains("ba")){
                    return true;
                }else{
                    return false;
                }
             }
            
        };
        List<String> answerList= new ArrayList<>();
        answerList.add("band");
        answerList.add("bake");
        answerList.add("bald");

        assertEquals(answerList,ListExamples.filter(testList,sc));
        
        
        
This input induces a failure.

@Test
    
    public void testFilter2(){
        
        List<String> testList= new ArrayList<>();

        testList.add("band");
        testList.add("hello");
        testList.add("madhav");

        StringChecker sc=new StringChecker() {
            public boolean checkString(String s) {
                if (s.contains("ba")){
                    return true;
                }else{
                    return false;
                }
             }
            
        };
        List<String> answerList= new ArrayList<>();
        answerList.add("band");
        assertEquals(answerList,ListExamples.filter(testList,sc));
    }
This input doesn't induce a failure.
 
Running of the two tests in vscode- 

<img width="1680" alt="Screenshot 2023-01-30 at 11 05 52 PM" src="https://user-images.githubusercontent.com/122562063/215690213-220d1f65-849d-4300-8ee8-b66141c753be.png">

Code before bug fix-

    class ListExamples {

    // Returns a new list that has all the elements of the input list for which
    // the StringChecker returns true, and not the elements that return false, in
    // the same order they appeared in the input list;
    static List<String> filter(List<String> list, StringChecker sc) {
        List<String> result = new ArrayList<>();
        for(String s: list) {
            if(sc.checkString(s)) {
                result.add(0,s);
            }
        }
        return result;
    }
 
Code after bug fix- 

    class ListExamples {

    // Returns a new list that has all the elements of the input list for which
    // the StringChecker returns true, and not the elements that return false, in
    // the same order they appeared in the input list;
    static List<String> filter(List<String> list, StringChecker sc) {
        List<String> result = new ArrayList<>();
            for(String s: list) {
                if(sc.checkString(s)) {
                    result.add(s);
                }
            }
        return result;
    }
 
This code had a very small bug- result.add(0,s) instead of result.add(s).

This resulted in the result array to show its elements in the order opposite of what was intended as elements were being

prepended in the new array instead of being appended.

## Part - 3 (Something new I learned)

I learned how to write and run junit tests in vscode in lab 2 which I didn't know before. This is a very useful tool for 

unit testing your code. I also learned how to debug a piece of code. We were given a bunch of methods with bugs and we had to write

Junit tests to figure out the bugs and fix it. These are extremely useful skills and I think will help me tremendously in the future.
