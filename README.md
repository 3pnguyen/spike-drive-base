# spike-drive-base

## Python code for advanced control over a LEGO SPIKE Prime Robot.

### Future improvements are planned from the original. (first repository so please be nice)

![Lego Sumo Robot](https://github.com/user-attachments/assets/ee1f8e5c-c7bc-49a2-9dbd-6699d1dd166d)
![Lego Test Robot + (Older) Sumo Robot](https://github.com/user-attachments/assets/d53f9aa7-05b6-46a4-96b5-5b000232539d)

Robots designed by me with a little help from my team

## ✨ More about the project

The code was written for my 8th grade adavanced robotics class to help make my team's robot (or any other SPIKE Prime robot) more accurate and reliable. Starting in 7th grade, it started as proportionate controllers to help the robot stay straight and turn more accurately. (done in block code) Transitioning to 8th, I would iterate many times until I landed onto a more advanced version. Then, I would learn Python, heavily bug fix and improve the code to be even more accurate, reliable, and functional. A graduation and a summer later, (9th as of now), I plan to improve the code from where I left off and hope to create a better foundation for anyone else who is working to improve their robot in FLL. (First Lego League)

(none of the other block code or Python code iterations could be documented on the repository because I didn't log my code at all back then... only a few Python versions exist before the version which I left off 8th grade with but I don't plan to add them)

This is what the "base", originial version can do:

* Create a reference point to where the code first starts to remove any errors that could have accumulated via the "drive straight"/"gyro straight" and the "gyro turn" individually
* Filter and cache sensor data to help remove sensor noise
* Use proportionate controllers to keep or turn the robot to the desired "heading" or angle relative to the refernce point
* Manage multiple "runs" or periods your robot may start and stop to do task(s) (for FLL, this could be doing a few missions)
* Even do sumo if your robot has a distance and color sensor

The reason I have this repository is to share my code for other people to use, (as said earlier), log versions, and to also to improve the code, partly since how I coded back then was a little weird. Before the code ended up getting more complex and longer in Python, I really wanted compact the code as much as I could. This was because the SPIKE Prime IDE (Integrated Development Environment, just a fancy place to code) does not let you hide or "fold" code that you can ignore, which is a pain when trying to work on the code for the runs when you would have to scroll to it. It wasn't bad then, but it did get worse overtime. When my code got longer, it was more about making it clearer to read rather than saving a few more lines. (and the techniques I used back then were not the best, believe me)

## ❗ Important

For an improved version of the code, check out the "improved" branch. I highly recommend it if you want to use it. The reason why it is not apart of the main branch is because I have not tested it.

## ✅ How to use this for your robot:

1. Download the llsp3 file for the code, whichever version you chooose
2. Go to the LEGO Education SPIKE website and choose SPIKE
3. Go to "Open Project" and open the llsp3 file
4. To actually use the code, you need to create an instance of the class "DriveAssist" which holds all of the methods or "SumoAssist" if you want to do sumo with your robot
5. After creating your instance and having your reference, your good to use any of the methods that the class provides

## 🤔 If you want contribute and help imporove the code:

* Do the same steps above; downloading and using the code
* Modify the code however you improve it
* Send it over here!

## 🪰 Did someone say bug?

* There have been tons of bugs with this code on the past and I am not 100% sure if there are bugs that still linger.
* If there is a bug, please sumbit it as an issue or however you do it. If you got an improvement to that bug, it would be great if you could send it over! (and don't forget to mention what bug it was)

## 👂 Speaking of "tons of bugs with this code on the past" and "bugs that still linger"...

It wouldn't hurt to mention some of them:

* The robot would jitter back in forth when doing a "gyro turn" near the targetted heading
* The robot is easily affected by gyro drift. If you are using the code for a long enough time the code will become inaccurate. The only way to fix this right now is to reset the relative point for the gyro.
* When using the sumo class and run method, the robot would sometimes retreat from the enemy even though there would be no reason to. For example, the robot may be in the middle of pushing the enemy, and then retreat for no reason!?
* When creating an instance of the two main classes, in the first and second argument, if you switched them around, the robot would work in reverse. (for example, if the first argument was port.A and the second port.B, (which are constants apart of the SPIKE environment) the robot would work correctly, but if you switched them around so it was port.B and port.A, the robot would not work as intended) Forward is backward and backward is forward, and probably at lot of other problems.

## ✍️ About the author

* I'm Ethan Nguyen and I created this hoping to help other people in FLL and Lego Robotics. I also wanted to improve my code, logging changes and fixing what the old version had bad or left out before
* My doing for all this roots to my passion for my robotics. Honestly, it's cool where it can get you in today's technology world
* When I was competeing in FLL with my team, I was one of the main coders, my other teamates worked on the FLL board and I was more in the back trying to innovate. We were the first team in our school district and our school to reach the finals of the competition. We didn't win anything but we still did pretty good. (22th place...) I mean, we won at least one trophy during qualifiers and reigionals. After FLL we did spring showdown (another LEGO robotics competition) and we placed top 10 in the first part and top 3 or 5 in the second part. Of course, I'm not a one man show and my team has contributed a lot. Thanks team!
* The LEGO robots at the top were designed by me and were used in spring showdown (one that was in the competition, and one that was for testing before the code was used on the main robot. The reason why the main robot does not look suited for spring showdown in the photo of it with the test robot was because it was after spring showdown and we were transitioning into sumo. I don't have many picures of the robots. The other picture was the final form of the sumo-ready robot that would win at the bracket for our local competition! My team helped design the black crowning so shoutout to them again!)
