# Lab Report - 5
## Madhav Bansal

## Researching Commands

1. find -name command option finds the files based on their name. (source of information ChatGpt)

```
MacBook-Pro-2:written_2 madhavbansal$ find ../written_2  -name "Bahamas-History.txt"
../written_2/travel_guides/berlitz2/Bahamas-History.txt
```
This command searches for the file with the name Bahamas-History.txt and returns the path of all the files that match the name.

```
MacBook-Pro-2:written_2 madhavbansal$ find ../written_2  -name "ch2.txt"
../written_2/non-fiction/OUP/Berk/ch2.txt
../written_2/non-fiction/OUP/Abernathy/ch2.txt
../written_2/non-fiction/OUP/Rybczynski/ch2.txt
../written_2/non-fiction/OUP/Fletcher/ch2.txt
```
This command searches for the file with the name ch2.txt and returns the path of all the files that match the name.

---

2. find -type command option searches for files based on their type( regular files, directories, etc.). (source of information ChatGpt)

```
find written_2 -type d
written_2
written_2/non-fiction
written_2/non-fiction/OUP
written_2/non-fiction/OUP/Berk
written_2/non-fiction/OUP/Abernathy
written_2/non-fiction/OUP/Rybczynski
written_2/non-fiction/OUP/Kauffman
written_2/non-fiction/OUP/Fletcher
written_2/non-fiction/OUP/Castro
written_2/travel_guides
written_2/travel_guides/berlitz1
written_2/travel_guides/berlitz2
```
This command option searches for all files of the type directory and returns their path.

```
MacBook-Pro-2:docsearch madhavbansal$ find written_2 -type f
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/non-fiction/OUP/Berk/ch7.txt
written_2/non-fiction/OUP/Abernathy/ch2.txt
written_2/non-fiction/OUP/Abernathy/ch3.txt
written_2/non-fiction/OUP/Abernathy/ch1.txt
.........
written_2/travel_guides/berlitz2/Bahamas-History.txt
written_2/travel_guides/berlitz2/Beijing-WhatToDo.txt
written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt
```

This command searches and returns all the regular files.

(I have not given all the file names as the output was too long)

---

3. find -size option searches for files based on thier size. (source of information ChatGpt)

```
MacBook-Pro-2:docsearch madhavbansal$ find written_2 -size +100k
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/travel_guides/berlitz1/WhereToIndia.txt
written_2/travel_guides/berlitz1/WhereToItaly.txt
written_2/travel_guides/berlitz1/WhereToMalaysia.txt
written_2/travel_guides/berlitz1/WhereToJapan.txt
written_2/travel_guides/berlitz1/WhereToFrance.txt
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
written_2/travel_guides/berlitz2/China-WhereToGo.txt
```
This command returns files with a size of more than 100 KiloBytes.

```
MacBook-Pro-2:docsearch madhavbansal$ find written_2 -size +200k
written_2/travel_guides/berlitz1/WhereToItaly.txt
written_2/travel_guides/berlitz1/WhereToFrance.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
```
This command returns files with a size of more than 200 KiloBytes.

---
4. find -mindepth option starts the search at a minimum depth in the directory tree. (source of information ChatGpt)

```
MacBook-Pro-2:docsearch madhavbansal$ find written_2 -type f -mindepth 4
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/non-fiction/OUP/Berk/ch7.txt
written_2/non-fiction/OUP/Abernathy/ch2.txt
written_2/non-fiction/OUP/Abernathy/ch3.txt
written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Abernathy/ch7.txt
written_2/non-fiction/OUP/Abernathy/ch6.txt
written_2/non-fiction/OUP/Abernathy/ch8.txt
written_2/non-fiction/OUP/Abernathy/ch9.txt
written_2/non-fiction/OUP/Abernathy/ch15.txt
written_2/non-fiction/OUP/Abernathy/ch14.txt
written_2/non-fiction/OUP/Rybczynski/ch2.txt
written_2/non-fiction/OUP/Rybczynski/ch3.txt
written_2/non-fiction/OUP/Rybczynski/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch3.txt
written_2/non-fiction/OUP/Kauffman/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch4.txt
written_2/non-fiction/OUP/Kauffman/ch5.txt
written_2/non-fiction/OUP/Kauffman/ch7.txt
written_2/non-fiction/OUP/Kauffman/ch6.txt
written_2/non-fiction/OUP/Kauffman/ch8.txt
written_2/non-fiction/OUP/Kauffman/ch9.txt
written_2/non-fiction/OUP/Kauffman/ch10.txt
written_2/non-fiction/OUP/Fletcher/ch2.txt
written_2/non-fiction/OUP/Fletcher/ch1.txt
written_2/non-fiction/OUP/Fletcher/ch5.txt
written_2/non-fiction/OUP/Fletcher/ch6.txt
written_2/non-fiction/OUP/Fletcher/ch9.txt
written_2/non-fiction/OUP/Fletcher/ch10.txt
written_2/non-fiction/OUP/Castro/chR.txt
written_2/non-fiction/OUP/Castro/chP.txt
written_2/non-fiction/OUP/Castro/chQ.txt
written_2/non-fiction/OUP/Castro/chB.txt
written_2/non-fiction/OUP/Castro/chC.txt
written_2/non-fiction/OUP/Castro/chA.txt
written_2/non-fiction/OUP/Castro/chV.txt
written_2/non-fiction/OUP/Castro/chW.txt
written_2/non-fiction/OUP/Castro/chM.txt
written_2/non-fiction/OUP/Castro/chZ.txt
written_2/non-fiction/OUP/Castro/chL.txt
written_2/non-fiction/OUP/Castro/chN.txt
written_2/non-fiction/OUP/Castro/chY.txt
written_2/non-fiction/OUP/Castro/chO.txt
```
This command only shows thw files at a minimum depth of 4 in the directory tree.

```
MacBook-Pro-2:docsearch madhavbansal$ find written_2 -type f -mindepth 5
```
This command only shows thw files at a minimum depth of 5 in the directory tree.

It has no output as there are no files at a minimum depth of 5 in the directory tree.

## Source of Information

I used ChatGpt for this information.

<img width="1470" alt="Screenshot 2023-03-13 at 1 16 27 PM" src="https://user-images.githubusercontent.com/122562063/224822381-62f6cb0d-8b38-41f8-ab59-0867608eb711.png">








