# Plugins installation and configuration

To start building your application with Flutter using IntelliJ IDEA, you must install Flutter and Dart plugins. The Flutter plugin is 
responsible for hot reload, running, debugging, and other developer workflows, while the Dart plugin carries out code analysis features:
code completion, validation, and so on. These plugins work in tandem.

## Plugins installation

To install the plugins:

1. Press ``Ctrl+Alt+S`` (Win, Linux) or ``⌘,`` (Mac OS) to open the **Settings** dialog and go to **Plugins**.
2. Click the **Browse repositories** button at the bottom of the window to view the list of available plugins.
3. Find the Flutter plugin using the search field and click **Install** on the right side of the window.
4. Click **Yes** when IntelliJ IDEA suggests to install the Dart plugin.
5. Close the Settings dialog by clicking **OK**.
6. Restart IntelliJ IDEA for the changes to take effect.

## Plugins configuration

Once you have installed the plugins, you must specify proper SDK paths.

### Flutter plugin configuration
1. Press ``Ctrl+Alt+S`` (Win, Linux) or ``⌘,`` (Mac OS) to open the **Settings** dialog and go to **Languages & Frameworks | 
Flutter**.
2. Specify the Flutter SDK path in the field at the top of the window. Once it is done, the current version is displayed.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img/flutter_sdk_path_1.png" alt="Inspector Toolbar" width="700"/>
</p>

3. Click **OK**.

### Dart plugin configuration
1. Press ``Ctrl+Alt+S`` (Win, Linux) or ``⌘,`` (Mac OS) to open the **Settings** dialog and go to **Languages & Frameworks | Dart**.
2. Specify the Dart SDK path in the field at the top of the window. Note that this path is actually inside of your Flutter SDK 
directory. For instance, if the Flutter SDK location is ``\src\flutter-sdk\flutter``, the Dart SDK location will be 
``\src\flutter-sdk\flutter\bin\cache\dart-sdk``. Once the path is specified, the current version is displayed.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img/dart_sdk_path_1.png" alt="Inspector Toolbar" width="700"/>
</p>

3. Click **OK**.

## Additional configuration

Now you are all set to start working on your Flutter projects in IntelliJ IDEA. However, it might be a sound practice to configure your 
environment thoroughly. To study possible settings you can use the ``Ctrl+Alt+S`` (Win, Linux) or ``⌘,`` (Mac OS) shortcuts to open the 
**Settings** dialog and type *Flutter* or *Dart* in the search field. Your IDE will display the plugins-specific settings, from color 
schemes to live templates.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/1_settings.png" alt="Settings" width="700"/>
</p>

### Flutter-specific settings
IntelliJ IDEA allows you to configure a number of Flutter-specific settings that help to customize your working environment. For 
instance, you can enable the hot reload performing or formatting code on save, enable verbose logging, and so on. To view these 
settings, open the **Settings** dialog and go to **Languages & Frameworks | Flutter**. Now you can select or clear checkboxes in the 
**App Execution**, **General**, and **Experiments** sections. Each item has got a short description, which facilitates configuring. 
> **Note:** Pay attention to the **Experiments** section that contains new features that are still under development. For instance, Live preview area in Flutter Outline visualizes your widgets rendering, which you might find rather useful.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/1_settings_flutter.png" alt="Settings" width="700"/>
</p>

### Dart-specific settings
Make sure that your Dart code style looks exactly as you need: open the **Settings** dialog and go to **Editor | Code Style | Dart**. 
Now you can switch between style tabs (**Dartfmt**, **Tabs and Indents**, **Spaces**, **Wrapping and Braces**, **Blank Lines**, and **Code Generation**) and modify the Dart code style according to your preferences.
<p align="center">
<img src="https://github.com/straw-wave/draft/blob/master/img_final/1_settings_dart.png" alt="Settings" width="700"/>
</p>

### Shortcuts
Shortcuts are time savers that have become an integral part of IntelliJ IDEA usage. Do not forget to explore the Keymap once your 
new plugins are installed (**Settings dialog | Keymap**). There is a good chance that shortkeys for **Hot Reload** or **Hot Restart** will be used often.

### Color schemes
Modify existing color schemes or create new ones to make sure that working with Dart and Flutter Log will be comfortable. To check the color schemes, open the Settings dialog and go to **Editor | Color Scheme** and select **Dart** of **Flutter**.

---

**Next:** While working on your Flutter application you will interact with [tool windows](https://github.com/straw-wave/draft/blob/master/content/tool-windows.md). Some of them will be familiar to developers who have already worked in IntelliJ IDEA, however there are new tool windows that are designed specifically for Flutter and Dart plugins.
