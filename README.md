# Fruit-Catcher-Assignment-by-Convergence-Concepts
Fruit Catcher Assignment by Convergence Concepts, given an assignment from the company to enhance the game  Assignment Brief: Improvise on the existing open-source content from Gamification.  Here’s the requirement.  -      Change the background image to a scene of a garden or park in Singapore  -      Change the fruits to local tropical fruits ie. durian, mango, rambutan etc.  -      Include a timer  -      Any exciting features to enhance the user’s experience.
Changes made, Basic Changes

Background image:
jungle.jpg > Images/gardensbythebayunsplashfreeimagebyMiguelSousa.jpg (from unsplash, free for use images by the public).
Change the code @ background.src to the new image.


Speed of the Basket:
Problem: Basket movement speed is too slow in my opinion,
Solution: from this.playerSpeed = 10; > this.playerSpeed = 50; 

Change the fruits:
 to local tropical fruits ie. durian, mango, rambutan etc.
Changes made, orange, apple, melon to rambutan, durian and mango. pngs.

Improvements to the game layout size:
Problem: Layout size feels small in my opinion
Solution: Made changes to the canvas width and height to suit the image too! Displaying Singapore's Gardens by the bay landscape.
Hence giving the players more time to navigate through and catch more fruits as compared to previous layout.

Include a timer,
contextBack.fillText("TIME LEFT: " +timeLeft, 1040, 50);  (for the display onscreen)
Added a timeleft function, timeLeft--,
timeLeft = 20;
timerId = setInterval(countdown, 1000);

Reset timeLeft countdown everytime pressed enter key during restart and on restarting program.
ADDED a timeout onscreen display, function countdown() {
               if (timeLeft == 0) {
                  clearTimeout(timerId);
                  contextBack.fillText("TIMEOUT ", 560, 530);
                  player.gameOver = true;
  
             } else {
              
                timeLeft--;
          }
        }



