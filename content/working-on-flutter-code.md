# Working on Flutter code
You can use well-known features of IntelliJ IDEA when working on Flutter projects. On top of it the Dart and Flutter plugins work in 
tandem to take care of multiple language and SDK-specific tasks, from code completion to hot reload. This collaboration and the 
framework assistance allow to improve your productivity. Moreover, there are tools that have been designed specifically for 
working on Dart and Flutter code.

## Flutter Outline
The core building blocks in Flutter applications are widgets (everything-is-a-widget concept), so developers work with these blocks a lot. That is why it is important to deliver a powerful tool that can help to manage widgets efficiently and ensure that the structure remains correct. To manage your widgets, use the Flutter Outline tool. To open it, click **Flutter Outline** on the right side of the main IDE window (alternatively, you can choose **View | Tool Windows | Flutter Outline** on the main menu). You can center you widgets, add padding, wrap widgets with columns and rows, extract methods, move widgets up and down, and remove them. To perform a required action, click a corresponding button on the toolbar: 
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_flutter_outline_toolbar.png" alt="Flutter Outline Toolbar" width="590"/>
</p>

**Flutter Outline** allows you to both view the structure of your application and to modify it, if necessary. When you use this tool, the IDE will make sure that the structure is correct, so you can avoid typos or forgotten symbols. For instance, you can center a widget using the Outline tool: 

1. Select a widget.
2. Click the **Center widget** button on the toolbar.
3. Perform **Hot Reload** to see the changes.

<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_center_widget.gif" alt="" width=""/>|<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_center_widget_demo.gif" alt="" width="340"/>|
--- | --- |

>**Note:** Click the <img src="https://github.com/straw-wave/draft/blob/master/img_final/4_filter.png" alt="" width="18"/> icon in the upper-right corner of the **Flutter Outline** tool window to enable the filtering to show only widgets.  

## Widget Management
In addition, IntelliJ IDEA offers alternative widgets management opportunities: you can add padding, remove a widget, swap it with its parent, wrap it with a new widget, and so on by using the ``Alt+Enter`` (Win, Linux) or ``⌘↩`` (Mac OS) shortcut in the Editor. This method also allows to save your time and it makes sure that the structure of your project remains valid.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_center_widget_2.png" alt="Center Widget" width="400"/>
</p>

## Converting
In case if you need to convert ``child`` to ``children``, there is a quick way to do it. Use the ``Alt+Enter`` (Win, Linux) or ``⌘↩`` (Mac OS) shortcuts to open the menu and choose the **Convert to children** option.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_convert.png" alt="Convert" width="400"/>
</p>

## Live Templates 
IntelliJ offers several Flutter Live Templates that simplify adding new widgets to your project, so you can create Stateless (``stless``), Stateful (``stful``), Stateful with AnimationController (``stanim``), and Inherited (``inh``) widgets much faster. To view the templates available out of the box press ``Ctrl+Alt+S`` (Win, Linux) or ``⌘,`` (Mac OS) to open the **Settings** dialog and go to **Editor | Live Templates**. Expand the **Flutter** or **Dart** sections to see the samples and modify them, if necessary.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_live_template.gif" alt="Intention Actions" width="400"/>
</p>

## Hot Reload
**Hot reload** is a feature that injects updated source code files into the running VM (or a connected device). To initiate hot reload click the <img src="https://github.com/straw-wave/draft/blob/master/img_final/4_hot_reload.png" alt="" width="18"/> icon (use the ``Ctrl+Back Slash`` (Win, Linux) or ``⌘\`` (Mac OS) shortcut) in the upper-right corner of 
the main IDE window. Alternatively, you can press ``Ctrl+S`` (``⌘S``) to **Save All** changes, which also results in displaying the 
latest changes. 
> Note: The first loading on a physical device might take some time.

## Reformatting Your Code
You can easily reformat your code to make sure the proper Dart style is used. To do so, use the **dartfmt** command: it is possible to 
find it using the Find Action dialog (use the ``Ctrl+Shift+A`` (Win, Linux) or ``⌘⇧A`` (Mac OS) shortcut) or choose the 
**Reformat Code with dartfmt** option from the right-click menu.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_dartfmt.png" alt="Reformat Code with dartfmt" width="500"/>
</p>

## Trailing commas
Using the trailing commas can be a good solution if your code includes multiple tree-shaped blocks. Add a trailing comma at the 
end of parameter lists in constructions that you want to keep the format. It will help the formatter to implement the proper number 
of line breaks for the Flutter code.

## Opening a module in another IDE
If you want to open a module to modify its code in another IDE, IntelliJ IDEA offers a smooth way to do it. Find the ``android`` folder
in your **Project** tool window, right-click it, then choose **Flutter | Open Android module in Android Studio** 
(the similar feature is available for the Xcode SDK as well).

## Comments from the Dart Analysis server
Curly brackets can be divided by many lines of code in your app, which makes it tricky to determine beginning and ending of a specific 
invocation. The IDE displays special comments denoting classes and widgets.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_comments.png" alt="System Comments" width="500"/>
</p>

## Flutter commands
Invoking Flutter commands can be done quickly: just click the required action at the top of the ``pubspec.yaml`` window. You can install referenced packages (the ``Packages get`` command), upgrade them to the latest version (the ``Packages upgrade`` command), upgrade the Flutter framework itself (the ``Flutter upgrade``), and validate the installed tools and check their versions (the ``Flutter doctor`` command).
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_packages_get.png" alt="Packages get" width="800"/>
</p>

## Packages
There are numerous open-source packages that you can use in your projects. Thus, when you add a package name into the dependencies list (``pubspec.yaml``), IntelliJ IDEA allows to pull the package into the project in an elegant way: just click **Packages get** at the top of the window. The console should display the output of the following kind:
```
Running "flutter packages get" in demo_project... 
Process finished with exit code 0
```

## Importing libraries
In case if a Dart library that is required in your project has not been imported yet, the IDE can perform this for you. Press ``Alt+Enter`` (Win, Linux) or ``⌘↩`` (Mac OS) and select the library you need.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_import_library.png" alt="Packages get" width="500"/>
</p>

## Postfix Completion
The Dart plugin comes with a number of **Postfix Completion** templates, so make sure to take a look at them. To see the list of templates press ``Ctrl+Alt+S`` (Win, Linux) or ``⌘,`` (Mac OS) to open the **Settings** dialog and go to **Editor | General | Postfix Completion**.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_postfix_completion.png" alt="Postfix Completion" width="700"/>
</p>

---

**Next:** [Run](https://github.com/straw-wave/draft/blob/master/content/running-apps.md) you project and see the result.

