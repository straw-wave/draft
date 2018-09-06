# Creating projects

To start working on a Flutter project in IntelliJ IDEA you can either create a new project, or create a new project that contains 
already existing source code files.

## Creating a new project
Your new project will open the Flutter plugin starter application template first.

1. Click **Create New Project** from the **Welcome** window or choose **File | New | Project** on the main menu.
2. Select **Flutter** in the menu, make sure that the Flutter SDK path is specified correctly, and click **Next**. 
You will be prompted to fill in a number of fields in the **New Project** window.
3. Type the project name. Note that a module name must be valid: lower case and underscores are acceptable.
4. Specify the directory where your project must be saved.
5. Add a project description (*optional*).
6. Select the type of a project you want to create. Project descriptions are presented below in the **New Project** window.
7. Type your organization domain.
8. Select the Android and iOS languages that you want to use in your project.
9. Select the **Create project offline** checkbox in case if the network connection is slow or you need to work offline.
10. Additionally it is possible to expand the **More Settings** section at the bottom of the window to adjust module-related settings. 
For instance, you can modify a module name, set up the module content root and module file parent directory, and select the preferable 
project format.
11. Click **Finish**.

|         |            |
| ------------- |:-------------:|
|<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_new_project.png" alt="Allowed values" width="590"/>|<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_new_project_2.png" alt="Allowed values" width="590"/>| 

## Creating a project containing existing source code files

1. Click **Create New Project** from the **Welcome** window or choose **File | New | Project** on the main menu. 
> **NOTE:** Do not use the **File | New | Project from existing sources** for your Flutter projects. Currently the Import Project feature
does not support the Flutter framework.
2. Select **Flutter** in the menu, make sure that the Flutter SDK path is specified correctly, and click **Next**.
3. Specify the location of the directory that contains the required Flutter source code files.
4. Click **Finish**. 

---

# Running your app

## Prerequisites

To run and test your application you must have either a connected device or a configured virtual device. You can check the status in the
**Flutter Device Selection** field in the upper-right corner of the main IDE window. In case if you have not added a device yet, you can 
do it with the help of the **Android Virtual Device (AVD) Manager**. To open it choose **Tools | Android | AVD Manager** on the main tool 
bar. You can create and configure a new virtual device that will be used for running your application. If you need to use the iOS 
simulator, make sure that your Xcode SDK is installed and configured properly. Alternatively, you can use a physical device. To check the 
connection use the ``flutter doctor`` command in the console: it will provide you with the data on your environment.

## Running application

To run your application and check its look-and-feel and performance, use the buttons in the upper-right corner of the main IDE window. 
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img/5_run_app_toolbar.png" alt="Allowed values" width="590"/>
</p>

- You can build your project, either by clicking a hammer button or by using the the ``Ctrl+F9`` (Win, Linux) or ``⌘F9`` (Mac OS) 
shortcuts.	
- Select the device that you want to use for running your app in the **Flutter Device Selection** field. 
- Configure your Run/Debug options. You can actually perform a fine tuning: set the entrypoint for your application, set additional 
command-line arguments, manage build flavor, and add tasks that should run before the launch.
- Run the project (use the ``Shift+F10`` (Win, Linux) or ``^R`` (Mac OS) shortcuts).
- Run the project in the **Debug mode** and study the console output to make adjustments, if necessary (use the ``Shift+F9`` (Win, Linux) or ``^D`` (Mac OS) shortcuts).
- You can also run your application with coverage to see and study the coverage measurement results. To check the current coverage 
configuration press ``Ctrl+Alt+S`` (Win, Linux) or ``⌘,`` (Mac OS) to open the **Settings** dialog and go to **Build, Execution, 
Deployemnt | Debugger | Coverage**.
- Click the **Profile** button to launch your application in a profile mode. You need this in case if you are using **Observatory** (a 
debugging and profiling tool shipped with the Dart SDK) for profiling your application.
- **Flutter Hot Reload** allows to apply the latest changes in a quick and easy way. Press ``Ctrl+Back Slash`` (Win, Linux) or ``⌘\`` 
(Mac OS) to view the changes implemented in the app right away.
- If necessary, you can attach a debugger to your application process.
- Stop the application.

---

**Next:** Flutter and Dart plugins offer a number of [testing and debugging tools](https://github.com/straw-wave/draft/blob/master/content/testing-and-debugging.md) that will help you improve your application.  

