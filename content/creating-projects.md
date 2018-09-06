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

**Next**: The development process begins. When your new application is ready for initial testing, [run it](https://github.com/straw-wave/draft/blob/master/content/running-app.md) to adjust its functions 
on-the-fly.
