# Running your app

## Prerequisites

To run and test your application you must have either a connected device or a configured virtual device. You can check the status in the
**Flutter Device Selection** field in the upper-right corner of the main IDE window. In case if you have not added a device yet, you can 
do it with the help of the **Android Virtual Device (AVD) Manager**. To open it choose **Tools | Android | AVD Manager** on the main tool 
bar. You can create and configure a new virtual device that will be used for running your application. If you need to use the iOS 
simulator, make sure that your Xcode SDK is installed and configured properly. Alternatively, you can use a physical device. To check the 
connection use the ``flutter doctor`` command in the console: it will provide you with the data on your environment.

## Running application

To run your application and check its look-and-feel and performance, you can use the buttons in the upper-right corner of the main IDE window. 
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img/5_run_app_toolbar.png" alt="Toolbar" width="590"/>
</p>

### Build Project
You can build your project either by clicking a hammer button or by using the the ``Ctrl+F9`` (Win, Linux) or ``⌘F9`` (Mac OS) 
shortcuts.	

### Flutter Device Selection
Select the device that you want to use for running your app

### Run/Debug Configurations 
Configure your Run/Debug options. You can actually perform a fine tuning: set the entrypoint for your application, set additional 
command-line arguments, manage build flavor, and add tasks that should run before the launch.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/5_run_debug_configuration.png" alt="Run/Debug Configuration" width="600"/>
</p>

### Run
Run your project (use the ``Shift+F10`` (Win, Linux) or ``^R`` (Mac OS) shortcuts).

### Debug
Run the project in the **Debug mode** and study the console output to make adjustments, if necessary (use the ``Shift+F9`` (Win, Linux) or ``^D`` (Mac OS) shortcuts).

### Run with coverage
Run your application with coverage to see and study the coverage measurement results. To check the current coverage 
configuration press ``Ctrl+Alt+S`` (Win, Linux) or ``⌘,`` (Mac OS) to open the **Settings** dialog and go to **Build, Execution, 
Deployemnt | Debugger | Coverage**.

### Profile
Launch your application in a profile mode. You need this in case if you are using **Observatory** (a debugging and profiling tool shipped with the Dart SDK) for profiling your application.
> **Note:** The Profile mode is not available on simulators or emulators because profiling on simulators is not representative of real performance.

### Flutter Hot Reload
This feature allows to apply the latest changes in a quick and easy way. Press ``Ctrl+Back Slash`` (Win, Linux) or ``⌘\`` 
(Mac OS) to view the changes implemented in the app right away.

### Attach Debugger
You can attach a debugger to your application process.

### Stop
Stop the application.

## Running application in Terminal
In addition, you can use **Terminal** in IntelliJ to run Flutter code using the ``flutter run``, ``flutter run --release``, ``flutter run --profile``, and ``flutter test`` commands. 
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/5_terminal.png" alt="Allowed values" width="900"/>
</p>

---

**Next:** Flutter and Dart plugins offer a number of [testing and debugging tools](https://github.com/straw-wave/draft/blob/master/content/testing-and-debugging.md) that will help you improve your application.  


Action | Description
--- | --- 
**Running application** | To run your application and check its look-and-feel and performance, you can use the buttons in the upper-right corner of the main IDE window. <p align="center"><img src="https://github.com/straw-wave/draft/blob/master/img/5_run_app_toolbar.png" alt="Toolbar" width="590"/></p>
**Building project** | You can build your project either by clicking a hammer button or by using the the ``Ctrl+F9`` (Win, Linux) or ``⌘F9`` (Mac OS) shortcuts.	
**Selecting Flutter device** | Select the device that you want to use for running your app
**Configuring running/debugging** | Configure your Run/Debug options. You can actually perform a fine tuning: set the entrypoint for your application, set additional command-line arguments, manage build flavor, and add tasks that should run before the launch. <p align="center"><img src="https://github.com/straw-wave/draft/blob/master/img_final/5_run_debug_configuration.png" alt="Run/Debug Configuration" width="650"/></p>
