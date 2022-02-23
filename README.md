# Action Network Frontend Engineer Take Home Assignment

This take home assignment is designed to allow you to demonstrate frontend skills. 

## Expectations and Deliverables

Our expectations are:

* There is no time limit or due date, though we expect this may take a couple of hours to accomplish.
* This is a skills test and a way to demonstrate your talents, so we do not expect the finished product to be production ready. Loose ends, hard coded things, hacks to save time, all acceptable, though bonus points if you highlight those in your code, in comments, or in your writeup and talk through a bit how you'd make them production ready.
* That said, we do expect to be able to run your work ourselves to see what you've done and how it functions.
* Your work should be licensed in a way that allows us to examine the code you wrote and run it so we can test out its functions for the purposes of our hiring process. We do not need ownership or the right to run it in production, though a permissive open source license like MIT would be fine here too.

Your deliverables are:

* A repository on GitHub (public or private) with your work, accomplishing the goals set out in the instructions below. Feel free to fork this repository if you'd like.
* Instructions for how to run your code ourselves and demonstrate the features. (Can be a readme type file in the repository if you want.)

Overall, this project should demonstrate your skills in the frontend, so please approach it in that spirit. It doesn't have to be perfect, this is definitely *not* a design test, so we're not going to judge you on how it looks, and it doesn't have to be "right" or be free of bugs and the like. But it should demonstrate what you can do.

When you are finished, email a link to your repository and instructions to your hiring contact. If you need our GitHub usernames to add to a private repository, we can provide those.

## Instructions and Goals

Your goal with this assignment is to write a simple browser-based game in the javascript framework of your choice. The goal of the game is for the player to get to 50 points while pressing the "roll" button the fewest number of times. Here are the rules and guidelines of the game application:

* Before playing, the player should enter their name, so the app can keep track of best scores. (Local storage is fine.)
* A button should allow for starting of a new game for the current player.
* Once in a game, when "roll" button is pressed, a number from 0-10 should be randomly generated and displayed to the player. This number represents the number of points the player receives for that roll.
* The UI should display the current number of points and well as the number of rolls that the player has made during their current game.
* Before a player rolls, they can optionally use a "power up." A power up allows the player to select if the next roll will be an even or an odd number. The player can only use this power up twice during a given game.
* A player only "wins" when their score sums exactly to 50. For example, if a player has 45 points, they need a 5 to win. A 6 will not count. (Up to you if overshooting the 50 point target means the player loses the game and has to start over, or the roll is simply thrown out, while adding to their roll count, and they are able to try again to get the "right" number to win.)
* After the player wins, their name is added to the "high score" board, sorted by number of rolls it took to win, lowest first. The high score board should keep track of the 5 best scores. It should persist even through page refreshes.
* If a player beats a high score, the UI should congratulate them.

Overall, this assigment aims to get a sense of your coding skill and comfort with modern frontend practices. As such, while we know that this can be implemented in a single javascript file, we are looking for a solution which demonstrates basic state tracking, use of discrete components, and design pattern best practices. As noted above, we do expect you to use at least one framework to organize your app.

Also note that building this with an eye towards future features and integration with a backend is a plus. For example, in the version of the game you are creating, the high scores and leader board may be kept locally, but in the future these scores may be kept on a global backend, enabling a global leaderboard, and we may want to adjust how many high scores are displayed when the game takes off. When building your solution, design it such a way that the implementation of the leader board can be easily swapped to use a backend API and display more than 5 leaders. A potential rough draft of the backend API might have the following endpoints:  

GET /api/getLeaders?count=5  
POST /api/addScore?user=foo&rolls=22

If you have any questions as you go, please don't hesitate to reach out to your hiring contact.

Good luck! We're looking forward to seeing your work!
