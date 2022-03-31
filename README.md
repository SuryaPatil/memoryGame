# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Surya Patil

Time spent: 2 hours spent in total

Link to project: (insert your link here, should start with https://glitch.com...)

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [x] Buttons use a pitch (frequency) other than the ones in the tutorial
* [x] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [ ] Computer picks a different pattern each time the game is played
* [x] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

-Extra features mentioned above that I have not completed.
-Scoreboard( lower score for higher number of mistakes, time it took to complete the game)

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
![] https://recordit.co/GZ36LDy9BL
![](https://recordit.co/oEMaUGUaZ6
![]https://recordit.co/edRzpOeXUQ
![](gif4-link-here)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 

    N/A

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

	One challenge I ran into was setting the user’s mistakes to 3. Initially, I had trouble understanding where exactly the program decided to end the game after just one mistake. I only knew that the code for this specific feature had to have been in the index.js file, since that is where I wrote all the logic. Numerous functions were in the index.js file, so it was difficult to find out which exact function controlled the continuity of the game. After looking back at the tutorial, I realized that the guess(btn) function was where I needed to tweak the code. However, the original program had no way of keeping track of the number of mistakes the user had made, because it simply ended after one mistake. Hence, I needed to make new variables for this situation. I created two new variables, guessesWrong and guessLimit. guessesWrong would keep track of the number of mistakes and would increment each time the user selected an incorrect button. guessLimit would be the number of mistakes the user makes before losing the game. Inside the else clause of the guess function,  I incremented. guessesWrong. Additionally, I had to create a nested conditional in the else clause of the guess function to check if guessesWrong was equal to guessesLimit. Having made all these adjustments, I was able to change the mistake limit to 3. 


3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

A large part of web development involves building full-stack applications, with both a backend and a frontend. Many web applications use a database to help with their backend. I am eager to learn more about how databases help developers build a backend for their web apps and how to incorporate databases into my own projects. I am also intersted in the diffrent options developers have when creating a databse. Developers can choose from SQLite, MongoDB, Amazon DynamoDB, and many other technologies. I am curious to learn why some deveolpers choose to use some technologies over others. Additionally, I know that APIs play a significant role in building web applications. However, I only have a vague understanding of what an API is and how to use one. If I were to learn more about web development, I would be interested in learning how APIs can help me achieve my goals. Lastly, few developers build web-applications by themselves. From hackathons to industry, web development is often done in large groups of people. I would like to become more familiar with how developers use tools such as Github, Trello, and other technologies to help collaborate with their peers. Overall, I am very early in my web-development journey and I can not wait to learn more.


4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

	I would implement many of the extra features listed in the README file. For example, I would want the playback to speed up after each turn. I believe this would make the game more engaging, since the user would have to play closer attention to each pattern. To accomplish this task, I would most likely have to adjust how I increment the clueHoldTime variable in the index.js file, since this variable controls how long each clue can be observed by the user. An additional feature I would like to implement is a scoreboard. A scoreboard would also provide a more engagin experience for the user, because it would allow them to compare themselves to other players and keep track of whether they are improving after each game. I would most likely create some space between the start buttons and the button area, and place the scoreboard here.




## Interview Recording URL Link

[My 5-minute Interview Recording]https://www.youtube.com/watch?v=XzLSxyxv3rk


## License

    Copyright Surya Patil

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
