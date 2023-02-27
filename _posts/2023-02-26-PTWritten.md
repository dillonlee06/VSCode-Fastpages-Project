---
toc: true
layout: post
categories: [CSP Assignments]
title: College Board Write Up
---

# Important links
- [Runtime Video](https://youtu.be/4FL82PGx8-U)
- [Simple Demo Video]()
- [Original CTP Plan](https://dillonlee06.github.io/VSCode-Fastpages-Project/csp%20assignments/2023/01/29/Psplanning.html)

# Row 1
> Requirements:
- Purpose: The features included in my contribution to the project help users learn and become familiar with the time it takes to charge one's electric car and includes the main cars from the brands Tesla, Lucid, Nio, and Rivian which are the all electric car manufacturers that our website covers. This information which therefore help users decide the benefits/harms of selecting a certain electric car, in terms of charging speeds.
- Video Explanation: The video shows how the user must first select one of the four electric car brands our organization covers which then takes the user to a page where it prompts them with a play button. After clicking the button, the user must use their cursor to drag their car into the intended parking space (square) where it then prompts the user to input a numerical value for time in minutes for how long they think it will take to charge the car to 100% from the random percentage it was at originally. After hitting submit, their score is then calculated and then a link is revealed to futher inform the user with other people's submitted experiences with their electric cars through clicking the reveal button. The user can also input their own experience with their electric car.

# Row 2
> Requirements:
- ![]({{site.baseurl}}/images/ptrow2.png "PT Row 2")
- Top segment of code shows the dictionary which is named "percentage_list" which represents the percentages and answers for the game
- Bottom segment of code uses the dictionary to get a random percentage which is the "00", "10", etc. in the dictionary as well as the answer (ans) which is the value assigned to the percentage in the dictionary

# Row 3
> Requirements:

# Row 4
> Requirements:

# Row 5
> Requirements:

# Row 6
> Requirements:
- Condition of first call: Tests what happens when someone tries to enter anything other than a number
- Result of first call/What is tested: Does not allow the answer to be submitted due to the input box type as numerical and if someone types "e" which is a constant, an error message pops up which was coded in the program
- Condition of second call: Tests what happens when a user tries to drag the car into the incorrect spot
- Result of second call/What is tested: The car is reset to the original spot and does not reveal the input box and guessing part of the game until it is dragged and dropped into the correct parking spot.