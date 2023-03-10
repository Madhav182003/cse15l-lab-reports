# Lab Report-4
## Madhav Bansal

# Step-1 Deleting existing forks

Go to the fork.

Go to settings and navigate to the Danger Zone and click delete repository.

<img width="1680" alt="Screenshot 2023-02-24 at 12 41 10 PM" src="https://user-images.githubusercontent.com/122562063/221542485-cfab4064-0db6-46af-975a-4c63a6ef6635.png">

verify that you want to delete.

# Step-2 Fork the Repository

open the github repository and press Fork.

<img width="1680" alt="Screenshot 2023-02-27 at 2 36 17 AM" src="https://user-images.githubusercontent.com/122562063/221542679-7f7fbda7-dd65-4929-a8e0-1b27df8166c8.png">


# Step-3

Start the Timer.

# Step-4 Log in to ieng6

Open terminal.

type command ssh cs15lwi23___@ieng6.ucsd.edu.

(replace ___ with your course specific account)

<img width="547" alt="Screenshot 2023-02-27 at 2 45 10 AM" src="https://user-images.githubusercontent.com/122562063/221543419-1acf68d9-3395-4700-a917-185c2a1fec45.png">

# Step-5 clone the fork.

Open the fork in your repository and copy the ssh link.

<img width="1680" alt="Screenshot 2023-02-27 at 2 47 05 AM" src="https://user-images.githubusercontent.com/122562063/221543756-334d551f-03c0-4b5b-9e3d-9e1903bf00bf.png">

Then Type git clone and press `< command-v >` to paste the ssh link.

Press `< Enter >` to clone the repository.

<img width="573" alt="Screenshot 2023-02-27 at 2 48 18 AM" src="https://user-images.githubusercontent.com/122562063/221544111-86516025-e969-4a1f-91c2-3a8433de13c3.png">

# Step-6 Run tests.

First I changed the directory to lab7 using the command cd lab7.

the I used the command ls to see the files.

Then I pressed `< ^R >` to open the search and typed javac to find the compile command and pressed `< up >< down >` to get 

the cursor to the end and changed the file to *.java to compile all the java files and pressed `< Enter >` to compile.

I the typed ls to see if the java files compiled. 

Then I pressed `< ^R >` to open the search and typed java to find the run command and pressed `< up >< down >` to get 

the cursor to the end and changed the file name to ListExamplesTests and pressed `< Enter >` to run the tests.


<img width="1680" alt="Screenshot 2023-02-27 at 2 52 14 AM" src="https://user-images.githubusercontent.com/122562063/221546470-c9a2c04c-ab60-4a68-8503-30ca95df28a1.png">

2 Tests ran and 1 failed.

# Step-7 Fixing the Code.

Type the command nano FileExamples.java to open the java file in a text editor nano in which you can edit.

<img width="1680" alt="Screenshot 2023-02-27 at 3 05 20 AM" src="https://user-images.githubusercontent.com/122562063/221547846-5931f56e-c25f-47d6-9349-147774b8bb25.png">

Then a screen with the code appears.

I pressed `< down >` arrow key 42 times, pressed the `< right >` key 12 times and pressed the `< delete >` key to change index1 to index2.

<img width="1680" alt="Screenshot 2023-02-27 at 3 04 50 AM" src="https://user-images.githubusercontent.com/122562063/221548266-7c6e6292-d7bc-44d2-9c85-710bc60f5d1a.png">

Then I pressed `< ^o >` and `< Enter >` to save the changes and `< ^x >` to exit nano.

# Step-8 Run the tests

I pressed `< ^R >` to open the search and typed javac to find the compile command and pressed `< Enter >` to compile.

Then I pressed `< ^R >` to open the search and typed java to find the run command and pressed `< Enter >` to run the tests.

<img width="570" alt="Screenshot 2023-02-27 at 3 10 01 AM" src="https://user-images.githubusercontent.com/122562063/221549018-337a399e-b36c-4561-9462-6ffd60ad8179.png">

2 tests ran and both passed.

# Step-9 Comitting and Pushing the changes

To commit you first have to make the changes available to commit.

So, I first typed `<git add>` .

Then I typed `<git commit -m "Fixed">` to commit the changes with the message Fixed.

Then I typed `<git push>` to push the changes to my repository.

<img width="1680" alt="Screenshot 2023-02-27 at 3 14 39 AM" src="https://user-images.githubusercontent.com/122562063/221549974-388eceb7-0747-4a97-8d2f-5a6ec5844675.png">























