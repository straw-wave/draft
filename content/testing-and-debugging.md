# Testing and debugging

Besides common debugging features that should be familiar to IntelliJ IDEA users, there are some tools that have been designed 
specifically for Dart and Flutter. Some of them run in background, like the Dart Analyzer tool, so you do not need to run the
``flutter analyze`` command. Thus, your code is being analyzed and the IDE points out possible mistakes and issues for you. Other new 
tools, for instance, include **Flutter Inspector** and **Observatory**. You can use them to test, analyze, and debug your application.

## Flutter Inspector

Widgets are used as the core building blocks in Flutter (everything-is-a-widget concept), so it was important to provide developers with 
a powerful tool for visualizing and exploring widget trees, which might actually get really busy. **Flutter Inspector** is the 
tool that helps to visualize, explore, and debug Flutter UIs. It helps to manage bidirectional mapping between an active Flutter UI and 
the corresponding visualization of the widgets tree and the Render Tree. Such approach allows you to follow this mapping into the source 
itself, so you can actually see where in the code (whether it is your code or the the framework code) a widget is being created or 
configured. This way, even the huge widgets tree can be handled in an elegant way: selecting a widget of your interest helps both to 
navigate at ease and to save time.

So, you have your application running and you want to inspect it, check the layouts, widgets, and performance. To open the tool, 
click **Flutter Inspector** on the right side of the main IDE window (alternatively, you can choose **View | Tool Windows | Flutter 
Inspector**). Use the toolbar to interact with elements of an app and to switch between Inspector tabs:

![Inspector Toolbar](https://github.com/straw-wave/draft/blob/master/img/5_inspector_toolbar.png)

You can start with the "Select Widget Mode". Click the button to activate this mode. Now you can select a widget that you are interested in, so when you interact with your device, you are not interacting with the application directly, but you can see which widget is responsible for a specific position on the screen. Now you can see the tree of widgets, the widget's position, and its properties. 
Tip: hover over a property value to see the list of allowed values.

|         |            |
| ------------- |:-------------:|
| ![Allowed values](https://github.com/straw-wave/draft/blob/master/img_final/5_allowed_values.png)|<img src="https://github.com/straw-wave/draft/blob/master/img_final/5_allowed_values_2.png" alt="Allowed values" width="600"/>| 
