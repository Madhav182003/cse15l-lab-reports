# Lab Report - 3
## Madhav Bansal

## Researching Commands

1. grep -r command option of grep recursively searches the directory and subdirectories (if any). (source of information ChatGpt)

```
grep -r "Lucayans" written_2

written_2/travel_guides/berlitz2/Bahamas-History.txt:Centuries before the arrival of Columbus, a peaceful Amerindian 
people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled 
up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the 
experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492.
Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed 
the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two 
weeks before sailing towards Cuba.

written_2/travel_guides/berlitz2/Bahamas-History.txt:The Spaniards never bothered to settle in the Bahamas, but the number of
shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, 
Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used 
to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold.
As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — 
in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.
```



This command recursively searched the directory for the string "Lucayans" and showed the paragraph within the file that contained it.




```
grep -r "tilted" written_2
written_2/non-fiction/OUP/Rybczynski/ch2.txt:Whimsy is absent from the tops of the 1970s office blocks around Bryant Park.
They look as if the architects had lopped them off on a whim: “I can do 40 floors, or 42, or 45. Just tell me when to stop.
” More recent skyscrapers around Bryant Park, no doubt emboldened by Philip Johnson’s Chippendale top on his AT&T Building,
have more animated crowns. The hipped roof of a Fifth Avenue Postmodern high-rise adorned with circles and squares peeks out above 
the library. The top of the Bertelsmann Building is a slender spike. The new Condé Nast office tower has tilted forms resembling speaker 
cabinets on its roof. Pretty tame stuff compared to the more fanciful crowns of the 1920s buildings—neo-Gothic spires, Romanesque tile roofs, 
copper domes. The 58 floors of 500 Fifth Avenue (at the corner of Fifth Avenue and 42nd Street), which was designed by Shreve & 
Lamb prior to the Empire State Building, step back dramatically as they reach the building’s apex. Spiky, wrought-iron finials enliven the
chateau-like roof of the Scientific American Building. An animated silhouette of black brick with gilded and red highlights crowns the Radiator
Building. According to Hood, the dramatic effect (floodlit at night) suggested a “pile of coal, glowing at the top.”

```



This command recursively searched the directory for the string "tilted" and showed the paragraph within the file that contained it.


---

2. grep -l command option of grep shows only the names of files that contain at least one matching line, not the matching lines themselves. (source of information ChatGpt)



```
grep -r -l "Italy" written_2
written_2/non-fiction/OUP/Castro/chP.txt
written_2/non-fiction/OUP/Fletcher/ch2.txt
written_2/non-fiction/OUP/Fletcher/ch9.txt
written_2/non-fiction/OUP/Rybczynski/ch2.txt
written_2/travel_guides/berlitz1/HistoryFrance.txt
written_2/travel_guides/berlitz1/HistoryGreek.txt
written_2/travel_guides/berlitz1/HistoryIstanbul.txt
written_2/travel_guides/berlitz1/HistoryItaly.txt
written_2/travel_guides/berlitz1/HistoryMadeira.txt
written_2/travel_guides/berlitz1/HistoryMallorca.txt
written_2/travel_guides/berlitz1/IntroItaly.txt
written_2/travel_guides/berlitz1/IntroLasVegas.txt
written_2/travel_guides/berlitz1/WhatToItaly.txt
written_2/travel_guides/berlitz1/WhereToEgypt.txt
written_2/travel_guides/berlitz1/WhereToFWI.txt
written_2/travel_guides/berlitz1/WhereToFrance.txt
written_2/travel_guides/berlitz1/WhereToGreek.txt
written_2/travel_guides/berlitz1/WhereToIstanbul.txt
written_2/travel_guides/berlitz1/WhereToItaly.txt
written_2/travel_guides/berlitz1/WhereToMadrid.txt
written_2/travel_guides/berlitz2/Algarve-History.txt
written_2/travel_guides/berlitz2/Athens-History.txt
written_2/travel_guides/berlitz2/Athens-WhatToDo.txt
written_2/travel_guides/berlitz2/Barcelona-WhereToGo.txt
written_2/travel_guides/berlitz2/California-WhereToGo.txt
written_2/travel_guides/berlitz2/Canada-History.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
written_2/travel_guides/berlitz2/Costa-History.txt
written_2/travel_guides/berlitz2/CostaBlanca-History.txt
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
written_2/travel_guides/berlitz2/Paris-WhereToGo.txt
written_2/travel_guides/berlitz2/Portugal-History.txt
written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt

```



The -l option only showed the names of the files that contained the string "Italy".




```
grep -r -l "Lucayans"  written_2
written_2/travel_guides/berlitz2/Bahamas-History.txt
```



The -l option only showed the name of the file that contained the string "Lucayans".




---




3. grep -c command option of grep shows only a count of the number of matching lines for each file. (source of information ChatGpt)




```
grep -c -r "India" written_2
written_2/non-fiction/OUP/Abernathy/ch1.txt:1
written_2/non-fiction/OUP/Abernathy/ch14.txt:0
written_2/non-fiction/OUP/Abernathy/ch15.txt:0
written_2/non-fiction/OUP/Abernathy/ch2.txt:0
written_2/non-fiction/OUP/Abernathy/ch3.txt:0
written_2/non-fiction/OUP/Abernathy/ch6.txt:0
written_2/non-fiction/OUP/Abernathy/ch7.txt:0
written_2/non-fiction/OUP/Abernathy/ch8.txt:0
written_2/non-fiction/OUP/Abernathy/ch9.txt:0
written_2/non-fiction/OUP/Berk/CH4.txt:5
written_2/non-fiction/OUP/Berk/ch1.txt:2
....
written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt:6
written_2/travel_guides/berlitz2/Vallarta-History.txt:1
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:0

```



This comand shows how many times the string "India" appeared in each file.
(I have not given the whole output here as it was too long.)




```
grep -c -r "Bahamas" written_2
written_2/non-fiction/OUP/Abernathy/ch1.txt:0
written_2/non-fiction/OUP/Abernathy/ch14.txt:0
....
written_2/travel_guides/berlitz2/Bahamas-History.txt:23
written_2/travel_guides/berlitz2/Bahamas-Intro.txt:11
written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt:16
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt:34
written_2/travel_guides/berlitz2/Bali-History.txt:0
written_2/travel_guides/berlitz2/Bali-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Bali-WhereToGo.txt:0
written_2/travel_guides/berlitz2/Barcelona-History.txt:0
written_2/travel_guides/berlitz2/Barcelona-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Barcelona-WhereToGo.txt:0
written_2/travel_guides/berlitz2/Beijing-History.txt:0
written_2/travel_guides/berlitz2/Beijing-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Beijing-WhereToGo.txt:0
written_2/travel_guides/berlitz2/Berlin-History.txt:0
written_2/travel_guides/berlitz2/Berlin-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Berlin-WhereToGo.txt:0
written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt:0
written_2/travel_guides/berlitz2/Bermuda-history.txt:0
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt:0
written_2/travel_guides/berlitz2/Budapest-History.txt:0
written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt:0
written_2/travel_guides/berlitz2/California-History.txt:0
written_2/travel_guides/berlitz2/California-WhatToDo.txt:0
written_2/travel_guides/berlitz2/California-WhereToGo.txt:0
written_2/travel_guides/berlitz2/Canada-History.txt:0
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:1
....

```




This comand shows how may times the string "India" appeared in each file.
(I have not given the whole output here as it was too long.)



---




4. grep -n command option of grep prefixes each line of output with the line number within the file. (source of information ChatGpt)





```
grep -r -n "Lucayans" written_2

written_2/travel_guides/berlitz2/Bahamas-History.txt:6:Centuries before the arrival of Columbus, a peaceful Amerindian 
people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled 
up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the 
experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492.
Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed 
the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two 
weeks before sailing towards Cuba.

written_2/travel_guides/berlitz2/Bahamas-History.txt:7:The Spaniards never bothered to settle in the Bahamas, but the number of
shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, 
Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used 
to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold.
As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — 
in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.

```




The -n command shows the line number of the line in which the string "Lucayans" is present within the file.





```
grep -r "tilted" written_2
written_2/non-fiction/OUP/Rybczynski/ch2.txt:20:Whimsy is absent from the tops of the 1970s office blocks around Bryant Park.
They look as if the architects had lopped them off on a whim: “I can do 40 floors, or 42, or 45. Just tell me when to stop.
” More recent skyscrapers around Bryant Park, no doubt emboldened by Philip Johnson’s Chippendale top on his AT&T Building,
have more animated crowns. The hipped roof of a Fifth Avenue Postmodern high-rise adorned with circles and squares peeks out above 
the library. The top of the Bertelsmann Building is a slender spike. The new Condé Nast office tower has tilted forms resembling speaker 
cabinets on its roof. Pretty tame stuff compared to the more fanciful crowns of the 1920s buildings—neo-Gothic spires, Romanesque tile roofs, 
copper domes. The 58 floors of 500 Fifth Avenue (at the corner of Fifth Avenue and 42nd Street), which was designed by Shreve & 
Lamb prior to the Empire State Building, step back dramatically as they reach the building’s apex. Spiky, wrought-iron finials enliven the
chateau-like roof of the Scientific American Building. An animated silhouette of black brick with gilded and red highlights crowns the Radiator
Building. According to Hood, the dramatic effect (floodlit at night) suggested a “pile of coal, glowing at the top.”

```





The -n command shows the line number of the line in which the string "tilted" is present within the file.

## Source of Information-

I used ChatGpt for the information.

<img width="1231" alt="Screenshot 2023-02-13 at 12 50 06 AM" src="https://user-images.githubusercontent.com/122562063/218412447-f0c7e7b9-513d-4f34-b678-de64e5041255.png">


