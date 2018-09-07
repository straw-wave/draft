# Working on Flutter code
You can use well-known features of IntelliJ IDEA when working on Flutter projects. On top of it the Dart and Flutter plugins work in 
tandem to take care of multiple language and SDK-specific tasks, from code completion to hot reload. This collaboration and the 
framework assistance allow to improve your productivity. Moreover, there are tools that have been designed specifically for 
working on Dart and Flutter code.

## Flutter Outline
The core building blocks in Flutter applications are widgets (everything-is-a-widget concept), so developers will work with these blocks 
a lot. That is why it is important to deliver a powerful tool that could help manage widgets quickly and efficiently and ensure that the 
structure remains correct. **Flutter Outline** is the right tool for these purposes. To open it, click **Flutter Outline** on the right 
side of the main IDE window (alternatively, you can choose **View | Tool Windows | Flutter Outline** on the main menu). To manage your widgets structure, use the toolbar:
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_flutter_outline_toolbar.png" alt="Flutter Outline Toolbar" width="590"/>
</p>

**Flutter Outline** allows you to both view the structure of your application and to modify it, if necessary. When you use this tool, the IDE will make sure that the structure is correct, so you can avoid typos or forgotten symbols. For instance, you can center a widget using the Outline tool: 

1. Select a widget.
2. Click the **Center widget** button on the toolbar.
3. Perform **Hot Reload** to see the changes.

<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_center_widget.gif" alt="" width=""/>|<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_center_widget_demo.gif" alt="" width="340"/>|
--- | --- |

Alternatively, you can use the ``Alt+Enter`` (Win, Linux) or  ``⌘↩`` (Mac OS) shortcuts to open the intention actions dialog and select the required action.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/4_center_widget_2.png" alt="Intention Actions" width="400"/>
</p>

This way, you can center you widgets, add padding, wrap widgets with columns and rows, extract methods, move widgets up and down, and 
remove them with the help of Flutter Outline. Additionally, you can enable the filtering to show only widgets.  

## Widget Management
In addition, IntelliJ IDEA offers alternative widgets management tool: you can add padding, remove a widget, swap it with its parent, 
wrap it with a new widget, and so on by using the Alt+Enter (Win, Linux) or ⌘↩ (Mac OS) shortcut in the Editor. This method also allows 
to save your time and it makes sure that the structure of your project remains valid.

![Managing widgets](https://github.com/straw-wave/draft/blob/master/img/3_widget_management.gif)

## Live Templates 
IntelliJ offers several Flutter Live Templates that simplify adding new Widgets to your project, so you can create Stateless, 
Stateful, Stateful with AnimationController, and Inherited Widgets much faster. To view the templates available out of the box 
press ``Ctrl+Alt+S`` (Win, Linux) or ``⌘,`` (Mac OS) to open the **Settings** dialog and go to **Editor | Live Templates**. 
Expand the **Flutter** or **Dart** sections to see the samples and modify them, if necessary.

![Live templates](https://github.com/straw-wave/draft/blob/master/img/3_live_template.gif)

## Hot Reload

**Hot reload** is a feature that injects updated source code files into the running VM (or a connected device). To initiate hot reload 
you can click the Lightning icon (use the ``Ctrl+Back Slash`` (Win, Linux) or ``⌘\`` (Mac OS) shortcut) in the upper-right corner of 
the main IDE window. Alternatively, you can press ``Ctrl+S`` (``⌘S``) to **Save All** changes, which also results in displaying the 
latest changes. 
> Note: The first loading on a physical device might take some time, but after that using hot reload and save should save time on 
updates.  

## Reformatting Your Code
You can easily reformat your code to make sure the proper Dart style is used. To do so, use the **dartfmt** command: it is possible to 
find it using the Find Action dialog (use the ``Ctrl+Shift+A`` (Win, Linux) or ``⌘⇧A`` (Mac OS) shortcut) or find the 
**Reformat Code with dartfmt** option in the right-click menu. Taking into consideration the fact that Flutter projects are based on 
Dart, it might be useful to create a new keyboard shortcut.

![Reformatting code](https://github.com/straw-wave/draft/blob/master/img/3_dartfmt.gif)

## Trailing commas
Using the trailing commas can be a good solution if your code includes busy tree-shaped blocks. Simply add a trailing comma at the 
end of parameter lists in constructions that you want to keep the format. It will help the formatter to implement the proper number 
of line breaks for the Flutter code.

## Opening a module in another IDE
If you want to open a module to modify its code in another IDE, IntelliJ IDEA offers a smooth way to do it. Find the ``android`` folder
in your **Project** tool window, right-click it, then choose **Flutter | Open Android module in Android Studio** 
(the similar feature is available for the Xcode SDK as well).

## Comments from the Dart Analysis server
Curly brackets can be divided by many lines of code in your app, which makes it tricky to determine beginning and ending of a specific 
invocation. The IDE displays special comments denoting classes and widgets.

![Dart Analysis server comments](https://github.com/straw-wave/draft/blob/master/img/3_dart_analysis_server_comments.png)

## Using packages
There are many open-source packages that you can use in your projects. Thus, when you add a package name into the dependencies list, IntelliJ IDEA allows to pull the package into the project in an elegant way: just click **Packages get** at the top of the window. The console should display the output of the following kind:
```
Running "flutter packages get" in demo_project... 
Process finished with exit code 0
```

![Packages get](https://github.com/straw-wave/draft/blob/master/img/3_packages_get.png)

## Importing libraries
When you create a new widget you can import the required Dart library in an easy way: just press ``Alt+Enter`` (Win, Linux) or ``⌘↩`` (Mac OS) and select the library you need. IntelliJ IDEA will perform the import for you.

---

**Next:** When the plugins are installed and the environment is configured, you can [create a new project](https://github.com/straw-wave/draft/blob/master/content/creating-projects.md) to start the development process.
