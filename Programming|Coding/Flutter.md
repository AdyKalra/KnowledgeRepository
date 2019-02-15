# [Flutter](https://flutter.io/)

[<img src="https://user-images.githubusercontent.com/1295961/45949308-cbb2f680-bffb-11e8-8054-28c35ed6d132.png" align="center" width="650">](http://flutter.io)


* Awesome Flutter - [Page](https://github.com/Solido/awesome-flutter)

### Usage
For more instructions on how to install flutter, look [here](https://flutter.io/docs/get-started/install)

* Install Git - Git for Windows 2.x, with the Use Git from the Windows Command Prompt option.
* Locate the file flutter_console.bat inside the flutter directory. Start it by double-clicking.
* Update the env variables - If the entry does exist, append the full path to flutter\bin
* Run flutter doctor in cmd
* Download and install [Android Studio](https://developer.android.com/studio/)
* Start Android Studio, and go through the ‘Android Studio Setup Wizard’. This installs the latest Android SDK, Android SDK Platform-Tools, and Android SDK Build-Tools, which are required by Flutter when developing for Android.
* Enable VM acceleration - [Windows10](https://www.quora.com/How-do-I-enable-hardware-acceleration-in-Windows-10) 

#### Set up the Android emulator
* Launch Android Studio > Tools > Android > AVD Manager and select Create Virtual Device. (The Android submenu is only present when inside an Android project.)
* Choose a device definition and select Next.
* Select one or more system images for the Android versions you want to emulate, and select Next. An x86 or x86_64 image is recommended.
* Under Emulated Performance, select Hardware - GLES 2.0 to enable hardware acceleration.
* Verify the AVD configuration is correct, and select Finish.
* In Android Virtual Device Manager, click Run in the toolbar. The emulator starts up and displays the default canvas for your selected OS version and device.

#### Google Developers
* Write Your First Flutter App [part 1](https://codelabs.developers.google.com/codelabs/first-flutter-app-pt1/#0)
* Write Your First Flutter App [part 2](https://codelabs.developers.google.com/codelabs/first-flutter-app-pt2/#0)

#### Observations
* Material app. Material is a visual design language that is standard on mobile and the web. Flutter offers a rich set of Material widgets.
* The main method uses fat arrow (=>) notation, Use fat arrow notation for one-line functions or methods.
* The app extends StatelessWidget, which makes the app itself a widget. In Flutter, almost everything is a widget, including alignment, padding, and layout.
* The Scaffold widget, from the Material library, provides a default app bar, a title, and a body property that holds the widget tree for the home screen. The widget subtree can be quite complex.
* A widget's main job is to provide a build method that describes how to display the widget in terms of other, lower-level widgets.
The body for this example consists of a Center widget containing a Text child widget. The Center widget aligns its widget subtree to the center of the screen.
* The pubspec file manages the assets for a Flutter app. In pubspec.yaml
* Stateless widgets are immutable, meaning that their properties can't change—all values are final.
* Stateful widgets maintain state that might change during the lifetime of the widget. Implementing a stateful widget requires at least two classes: 1) a StatefulWidget class that creates an instance of 2) a State class. The StatefulWidget class is, itself, immutable, but the State class persists over the lifetime of the widget.
* ListView's builder factory constructor allows you to build a list view lazily, on demand.
