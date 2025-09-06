# spike-drive-base

## ❓ Info

* This branch of the repository holds the updated versions of the original code that is in the main branch. This version of the code will be way cleaner and more robust compared to the original version. If you want to use this code, I recommend that you use this version.
* Using this code for yourself is the same process as for the original version.
* Of course, future updates are still planned.
* None of the versions have been tested so far, which is why there are multiple files for the same code. Each version is based off of the previous one, down to the original and tested version.
* Some of the updated version may fix the bugs from the original version.

## 🛠️ Changes

### 1️⃣ Update 1

* The code has been de-compacted, making it easier to read and look at but in turn takes up more lines.
* In the DriveAssist class, there is now a "reset_gyro" method to reset the relative point/heading for the robot. Before, this was exclusive to the GUI method. This means that you don't have to rely on the GUI method for the code if you don't want to.

### 2️⃣ Update 2

* The second class inherits the first class now, unlike how it used to be before. I didn't know about inheritance then, so this change fixes that. (The second class used to reference an instance to the first class, yuck)
* Any nested functions have a "_" in front of them now.
* The code has decompressed a little more because I "missed a spot".
* More documentation has been added to the code.

### 3️⃣ Update 3

* The drive straight/straight method has an acceleration argument. You can override the straight method to have less/more acceleration when needed.
* The drive straight/straight method uses a PID controller instead of a P controller.
* The DriveAssist class now has nested classes for a moving median filter, PID controller, and P controller. Any code using any of those controllers and filters now uses those classes.
* The moving median filter class comes with a check_stable_value method that returns a value if the value has enough frequency in the history list. The run method in the SumoAssist class uses this to make the state transitions more reliable. (hopefully)
