---
toc: true
layout: post
categories: [CSP Assignments]
title: College Board Write Up
---

# Important links
- [Runtime Video](https://youtu.be/4FL82PGx8-U)
- [Demo Video of Project](https://youtu.be/xeBE2QWRKNo)
- [Original CTP Plan](https://dillonlee06.github.io/VSCode-Fastpages-Project/csp%20assignments/2023/01/29/Psplanning.html)

# Row 1 (3. a.)
> Requirements:
- [Demo Video of Project](https://youtu.be/xeBE2QWRKNo)
- (3. a. i. ) Purpose: The features included in my contribution to the project help users learn and become familiar with the time it takes to charge one's electric car and includes the main cars from the brands Tesla, Lucid, Nio, and Rivian which are the all electric car manufacturers that our website covers. This information which therefore help users decide the benefits/harms of selecting a certain electric car, in terms of charging speeds.
- (3. a. ii.) Video Explanation: The program allows the player to park their electric car into a specified electric charging parking space to then charge their car by predicting how long it will take them to charge. They will then get a score and be prompted to go to a new page with information about electric car charging (CRUD/backend) and even input their own experience (if they have any) with electric car charging.
- (3 .a .iii.) Input Explanation: The video shows how the user must first select one of the four electric car brands our organization covers which then takes the user to a page where it prompts them with a play button. After clicking the button, the user must use their cursor to drag their car into the intended parking space (square) where it then prompts the user to input a numerical value for time in minutes for how long they think it will take to charge the car to 100% from the random percentage it was at originally. After hitting submit, their score is then calculated and then a link is revealed to futher inform the user with other people's submitted experiences with their electric cars through clicking the reveal button. The user can also input their own experience with their electric car.

# Row 2 (3. b.)
> Requirements:
- (3 .b. i.) and (3.b.ii.)
- ![]({{site.baseurl}}/images/ptrow2.png "Dictionary and Use of Dictionary")
- (3 .b. iii.) Top segment of code shows the dictionary which is named "percentage_list" which represents the percentages and answers for the game
- (3 .b. iv.) Bottom segment of code uses the dictionary to get a random percentage (simple percentage, not meant to be a complex game) which is the "00", "10", etc. in the dictionary as well as the answer (ans) which is the value assigned to the percentage in the dictionary

# Row 3 (3.b.v.)
> Requirements:
- The list manages complexity by easily taking all the simple percentages that I want, and compiling it all into one spot with the values of time in minutes which represents the time it will take to charge the car from that percentage. Without the use of this list, I would have to use the random math function to take a number between 0 and 99 and then make sure that it is divisible by 10 (as I want to keep the numbers simple for users) using a loop of some sorts. And then on top of that, I would have to figure out an extravagant formula to put in the program for determining the answer. My code is much simpler though as it is easy to just take a random instance from the list and assign variables for the percentage and answer in just four simple lines of code rather than potentially having to use a loop and other mathematical functions.

# Row 4 (3.c.)
> Requirements:
- (3.c.i.) ![]({{site.baseurl}}/images/ptrow4.1.png "Procedure")
- (3.c.ii.)![]({{site.baseurl}}/images/ptrow4.2.png "Procedure Call")
- (3.c.iii.) The procedure called "add_row" is used to add a row of data from my database of charging times into a table containing a certain electric car and a inputted charging time which any user could input. This gives users an idea of what other people have experienced in term of charging their different electrical cars and with that provided information, help themselves decide on what car they want to potentially look to buy in the future.

# Row 5 (3.c.iv.)
> Requirements:
- 

# Row 6
> Requirements:
- Condition of first call: Tests what happens when someone tries to enter anything other than a number
- Result of first call/What is tested: Does not allow the answer to be submitted due to the input box type as numerical and if someone types "e" which is a constant, an error message pops up which was coded in the program
- Condition of second call: Tests what happens when a user tries to drag the car into the incorrect spot
- Result of second call/What is tested: The car is reset to the original spot and does not reveal the input box and guessing part of the game until it is dragged and dropped into the correct parking spot.