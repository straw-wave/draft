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
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/5_inspector_toolbar_2.png" alt="Inspector Toolbar"/>
</p>

The following features are at your disposal: 

- **Toggle Select Widget Mode**: Select any widget in your project to inspect it. 
- **Refresh Widget Info**: A quick information updating.
- **Toggle Debug Paint**: This mode adds debug painting in your application to help you understand how widgets are laid out on the screen.
- **Toggle Platform Mode**: Switch between Android and iOS platform rendering to test platform-specific rendering without having to use two devices.
- "Toggle Performance Overlay": This tool displays the GPU & CPU threads performance graphs and allows you to analyze the current situation and improve the performance.
- "Open Timeline View": Analyze the activity statistics of the application on-the-fly.
- "Open Observatory": Open Observatory, a debugging and profiling tool shipped with the Dart SDK. 
- "Show Paint Baselines": Enable this feature the see a line each RenderBox will paint at its baseline.
- "Enable Repaint Rainbow": This option will show rotating colors on layers when repainting.
- "Enable Slow Animations": Slow your animations down, so you can perform visual inspection.
- "Hide Debug Banner": It is possible to hide the "Debug" banner that is displayed in the upper-right corner of your application by default when it is run in a debug mode.
- "Auto horizontal scroll": Enabling this feature might be useful if your widget structure is deep. When you scroll down, the IDE will pefrorm the horizontal scroll for you automatically.
- "Highlight nodes displayed in both trees".

You can start with the **Select Widget Mode**. Click <img src="https://github.com/straw-wave/draft/blob/master/img_final/5_select_widget_mode.png" alt="Select Widget Mode" width="18"/> button to activate this mode. Now you can select a widget that you are interested in, so when you interact with your device, you are not interacting with the application directly, but you can see which widget is responsible for a specific position on the screen. Now you can see the tree of widgets, the widget's position, and its properties. 
>**Tip:** hover over a property value to see the list of allowed values. When you perform a hot reload, the Inspector will update the widget properties accordingly.

|         |            |
| ------------- |:-------------:|
| ![Allowed values](https://github.com/straw-wave/draft/blob/master/img_final/5_allowed_values.png)|<img src="https://github.com/straw-wave/draft/blob/master/img_final/5_allowed_values_2.png" alt="Allowed values" width="590"/>| 

You have checked the widget's position and its properties, and in case if there is a problem with rendering of a UI element, you can switch to the **Render Tree** tab. Note that the **Widgets** and **Render Tree** tabs are connected, which means that if you have selected a widget and switch between tabs, you will get the data about the same widget. 
>**Tip:** If you have animations in your application, the Render Tree will display the values being changed on-the-fly. 

|         |            |
| ------------- |:-------------:|
|<img src="https://github.com/straw-wave/draft/blob/master/img_final/5_widgets-render_tree_1.png" alt="Allowed values" width="590"/>|<img src="https://github.com/straw-wave/draft/blob/master/img_final/5_widgets-render_tree_2.png" alt="Allowed values" width="590"/>| 

Use the **Debug Paint** mode to understand how your widgets are laid out on the screen. Click <img src="https://github.com/straw-wave/draft/blob/master/img_final/5_debug_paint.png" alt="Debug Paint" width="18"/> button to activate this mode.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/5_debug_paint_mode.png" alt="Debug Paint" width="300"/>
</p>

IntelliJ IDEA allows developers to make sure that the application works well on different platforms. To check the functionality and look-and-feel click the Platform Mode button. Now you can compare the properties and find the source of possible issues.

## Performance Overlay

The performance overlay displays the GPU & CPU threads performance graphs and allows you to analyze the current situation and improve the performance. Basically, if you are not astisfied with how smooth your application works, this tool should help. IntelliJ IDEA offers a simple implementation: click <img src="https://github.com/straw-wave/draft/blob/master/img_final/5_performance_overlay.png" alt="Performance Overlay" width="18"/> button in the Flutter Inspector tool window. Now you can test your application and check the performance statistics on the screen.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/5_performance_mode.png" width="300"/>
</p>

## Observatory and Timeline

Observatory is a debugging and profiling tool that provides profiling, examining the heap, and displaying code coverage. To open **Observatory**, you must run your application and click <img src="https://github.com/straw-wave/draft/blob/master/img_final/5_observatory_button.png" alt="Observatory" width="18"/> button (it is available in the **Run** or **Flutter Inspector** tool windows). 
  * Use **Observatory** to look inside a running Dart virtual machine and to get the current statistics about memory leaks, check which lines of code have been executed, and so on. 
  * **Timeline** is a tool that allows you to capture the stack snapshot.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/5_observatory.png" width=""/>
</p>

## Dart Analysis Tool Window

This tool window allows to monitor issues that might arise during the project development. The performance of this feature is based on the [Dart Analysis server](https://github.com/straw-wave/draft/blob/master/content/tool-windows.md#dart-analysis-tool-window), a local server that provides the essential data and functionality for the IDE: code completion, structure view, warnings, syntax highlighting and so on.

In the the **Dart Analysis** tool window you can:
  * Sort the errors by severity or location.
  * Group errors by severity.
<img src="https://github.com/straw-wave/draft/blob/master/img_final/5_dart_analysis_1.gif" alt="" width="590"/>  
 
 * Use the **Dart Problems Filter** to filter out some error messages if necessary.
 <img src="https://github.com/straw-wave/draft/blob/master/img_final/5_dart_analysis_2.gif" alt="" width="590"/>
 
  * Determine the precise location of an issue and move to it.
  * Identify the type of an issue (there can be errors, warnings, or hints).
  * Enable the **Autoscroll to Source** feature that allows to get to the issue in a quick way.
  * Restart the Dart Analysis Server.

