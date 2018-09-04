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

## Initial plugins configuration

Once you have installed the plugins, you must specify proper SDK paths.

### To configure the Flutter plugin:
1. Press ``Ctrl+Alt+S`` (Win, Linux) or ``⌘,`` (Mac OS) to open the **Settings** dialog and go to **Languages & Frameworks | 
Flutter**.
2. Specify the Flutter SDK path in the field at the top of the window. Once it is done, the current version shall be displayed.
![Flutter SDK Path](https://github.com/straw-wave/draft/blob/master/img/flutter_sdk_path_1.png)
3. Click **OK**.

### To configure the Dart plugin:
1. Press ``Ctrl+Alt+S`` (Win, Linux) or ``⌘,`` (Mac OS) to open the **Settings** dialog and go to **Languages & Frameworks | Dart**.
2. Specify the Dart SDK path in the field at the top of the window. Note that this path is actually inside of your Flutter SDK 
directory. 
For instance, if the Flutter SDK location is ``\src\flutter-sdk\flutter``, the Dart SDK location will be 
``\src\flutter-sdk\flutter\bin\cache\dart-sdk``. Once the path is specified, the current version should be displayed.
![Dart SDK Path](https://github.com/straw-wave/draft/blob/master/img/dart_sdk_path_1.png)
3. Click OK.

## Additional plugins configuration

Now you are all set to start working on your Flutter projects in IntelliJ IDEA. However, it might be a sound practice to configure your 
environment thoroughly. To study possible settings you can use the ``Ctrl+Alt+S`` (Win, Linux) or ``⌘,`` (Mac OS) shortcuts to open the 
**Settings** dialog and type Flutter or Dart in the search field. Your IDE will display the plugins-specific settings, from color 
schemes to live templates. Here are some things to pay attention to in this dialog.

### Flutter-specific settings
IntelliJ IDEA allows you to configure a number of Flutter-specific settings that help to customize your working environment. For 
instance, you can enable the hot reload performing or formatting code on save, enable verbose logging, and so on. To view these 
settings, open the **Settings** dialog and go to **Languages & Frameworks | Flutter**. Now you can select or clear checkboxes in the 
**App Execution**, **General**, and **Experiments** sections. Each item has got a short description, which facilitates configuration. 
Pay attention to the Experiments section that contains new features that are still under development. For instance, Live preview area 
in Flutter Outline visualizes your widgets rendering, which you might find rather useful.

### Dart-specific settings
Make sure that your Dart code style looks exactly as you need: open the **Settings** dialog and go to **Editor | Code Style | Dart**. 
Now you can switch between style tabs (**Dartfmt**, **Tabs and Indents**, **Spaces**, and so on) and modify the Dart code style 
according to your preferences.

### Shortcuts
Shortcuts are time savers that have become an integral part of IntelliJ IDEA usage. Do not forget to explore the Keymap once your 
new plugins have been installed (**Settings dialog | Keymap**).

### Color schemes
Modify existing color schemes or create new ones to make sure that working with Dart and Flutter Log will be as comfortable as 
possible. To check the color schemes, open the Settings dialog and go to **Editor | Color Scheme** and select **Dart** of **Flutter**.
