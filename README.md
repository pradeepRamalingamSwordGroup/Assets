# TransitNet SGS MobileApp

**TNet Mobile** Application aims to extend the range of services provided by TNet to their customers.      
Its main objective is to facilitate the transfer of commercial documents related to goods placed under Transit Procedures from the truck driver to the people responsible for transit declarations completion and processing.      
Other important objectives are to facilitate communication between drivers, SGS clients and SGS client centers and in this first version to introduce the possibility for SGS clients to check the status of their operations as well as their prepaid account.


# Development

## Flutter

Flutter is used to develop the TransitNet Mobile App, supporting iOS and Android operating system on both mobile and tablet devices.      
**Flutter** is an open-source UI software development kit created by Google. It is used to develop cross platform applications for Android, iOS, Linux, macOS, Windows, Google Fuchsia and the web from a single codebase


## Dart (programming language)

**Dart** is a programming language designed for client development, such as for the web and mobile apps. It is developed by Google and can also be used to build server and desktop applications.      
It is an object-oriented, class-based, garbage-collected language with C-style syntax. It can compile to either native code or JavaScript, and supports interfaces, mixins, abstract classes, reified generics and type inference.

# Setting up development environment

## Windows

Flutter SDK Install Guide - [Windows](https://docs.flutter.dev/get-started/install/windows)

## MacOS

Flutter SDK Install Guide - [MacOS](https://docs.flutter.dev/get-started/install/macos)

## Linux

Flutter SDK Install Guide - [Linux](https://docs.flutter.dev/get-started/install/linux)


> Note

```` 
* To be able to generate iOS builds or to debug on an iOS device, MacOS environment is required 
* Cannot compile for iOS on a Windows/Linux development environment 
````   


# IDE

There are numerous IDE's available to work on flutter projects. Few of the popular ones are listed below.

- [Android Studio](https://docs.flutter.dev/get-started/editor?tab=androidstudio)
- [VS Code](https://docs.flutter.dev/get-started/editor?tab=vscode)
- [Emacs](https://docs.flutter.dev/get-started/editor?tab=emacs)

After setting up the IDE, make sure you have the necessary plugins installed.

> To verify the setup run the following command to see if there are any platform dependencies that are incomplete

````flutter doctor````


For example:      
[-] Android toolchain - develop for Android devices      
• Android SDK at D:\Android\sdk      
**✗ Android SDK is missing command line tools; download from https://goo.gl/XxQghQ** • Try re-installing or updating your Android SDK,      
visit https://docs.flutter.dev/setup/#android-setup for detailed instructions.


# Setting up the project

After setting up the environment, setup the project by following the below mentioned steps.

**Step 1:**

Download or clone this repo by using the link below:    
``` https://swordsuisse@dev.azure.com/swordsuisse/SGS%20TransitNet/_git/SGS%20TransitNet ```

**Step 2:**

Go to project root and execute the following command in console to get the required dependencies:    
``` flutter pub get ```

**Step 3:**

This project uses libraries that works with code generation, execute the following command to generate files:    
``` flutter pub run build_runner build --delete-conflicting-outputs ```

**Step 4:**

To run the project, execute the following command:    
``` flutter run ```


# Libraries & Plugins

* [Path Provider](https://pub.dev/packages/path_provider) (Flutter plugin to get commonly used locations on the filesystem)
* [Shared Preferences](https://pub.dev/packages/shared_preferences) (Flutter plugin for reading and writing simple key-value pairs. Wraps NSUserDefaults on iOS and SharedPreferences on Android)
* [Provider](https://github.com/rrousselGit/provider) (State Management)
* [DropdownSearch](https://pub.dev/packages/dropdown_search) (Simple and robust Searchable Dropdown with item search feature)
* [Tuple](https://pub.dev/packages/tuple) (A library providing a tuple data structure)
* [http](https://pub.dev/packages/http) (A composable, Future-based library for making HTTP requests)
* [Flutter EasyLoading](https://pub.dev/packages/flutter_easyloading) (A clean and lightweight loading/toast widget)
* [JWT Decoder](https://pub.dev/packages/jwt_decoder) (Library to decode json web token)
* [Flutter SVG](https://pub.dev/packages/flutter_svg) (An SVG rendering and widget library for Flutter)
* [Firebase Core](https://pub.dev/packages/firebase_core) (Flutter plugin for Firebase Core, enabling connecting to multiple Firebase apps)
* [Firebase Messaging](https://pub.dev/packages/firebase_messaging) (Flutter plugin for Firebase Cloud Messaging, a cross-platform messaging solution)
* [Flutter Local Notifications](https://pub.dev/packages/flutter_local_notifications) (A cross platform plugin for displaying and scheduling local notifications)
* [URL Launcher](https://pub.dev/packages/url_launcher) (Flutter plugin for launching a URL)
* [Barcode Widget](https://pub.dev/packages/barcode_widget) (Barcode generation widget for Flutter)
* [Dotted Border](https://pub.dev/packages/dotted_border) (A flutter package to easily added dotted borders around widgets)
* [Map Launcher](https://pub.dev/packages/map_launcher) (Flutter plugin to find available maps installed on a device and launch them)
* [Stacked](https://pub.dev/packages/stacked) (An architecture and widgets for an MVVM inspired architecture in Flutter)
* [PackageInfoPlus](https://pub.dev/packages/package_info_plus) (Flutter plugin for querying information about the application package)
* [Drift](https://pub.dev/packages/drift) (Drift is a reactive library to store relational data in Dart and Flutter applications)
* [drift_db_viewer](https://pub.dev/packages/drift_db_viewer) (A package to view the drift database from within the app)
* [sqlite3_flutter_libs](https://pub.dev/packages/sqlite3_flutter_libs) (Flutter plugin to include native sqlite3 libraries with your app)
* [Path](https://pub.dev/packages/path) (A string-based path manipulation library)
* [Connectivity Plus](https://pub.dev/packages/connectivity_plus) (Flutter plugin for discovering the state of the network connectivity)
* [Permission Handler](https://pub.dev/packages/permission_handler) (This plugin provides a cross-platform API to request and check permissions)
* [PDFx](https://pub.dev/packages/pdfx) (Flutter plugin to render & show PDF files)
* [File Picker](https://pub.dev/packages/file_picker) (This plugin allows to use native file explorer)
* [Permission Handler](https://pub.dev/packages/permission_handler) (This plugin provides a cross-platform API to request and check permissions)
* [PDFx](https://pub.dev/packages/pdfx) (Flutter plugin to render & show PDF files)
* [File Picker](https://pub.dev/packages/file_picker) (This plugin allows to use native file explorer)
* [intl](https://pub.dev/packages/intl) (This plugin helps in internationalization/localization)
* [Flutter Location Plugin](https://pub.dev/packages/location) (Flutter plugin to easily handle realtime location)


# Folder Structure

Here is the core default folder structure which flutter provides.


``` 
TransitNetMobile/ 
|- android 
|- assets 
|- ios 
|- lib 
|- test 
``` 


Here is the folder structure for the main project files which would be under `lib`


``` 
lib/ 
|- app/ 
|- app_constant/ 
|- helpers/ 
|- models/ 
|- repositories/ 
|- utils/ 
|- view_models/ 
|- widgets/ 
|- main.dart 
```


### app

This is a simple `Service Locator` for Dart and Flutter projects.

### app_constant

All the application level constants are defined in their respective files. This directory contains the constants for `theme`, `strings`, and `country info list`.


``` 
constants/ 
|- app_constants.dart 
|- country_list.dart 
|- theme_constants.dart 
```


### helpers

Contains the `helper classes` required for the app functions


``` helpers/ 
|- api_helper/    
	|- response_models/
|- connectivity_helper/ 
|- db_helper/    
	|- dbModels/ 
|- global_snackbar_helper/ 
|- localization_helper/ 
|- location_helper/ 
|- prefs_helper/ 
|- push_notification_helper/ 
|- synchronization_helper/ 
``` 


> api_helper => Helper classes for REST API calls, error handling, response models
> connectivity_helper => Helper classes for verifying the device connectivity
> db_helper => Helper classes for database and extended models of database tables
> global_snackbar_helper => Helper class to display toast message globally
> localization_helper => Helper class to handle app localization
> prefs_helper => Helper class to manage app preferences and other data
> push_notification_helper => Helper class to manage push notifications
> synchronization_helper => Helper class to sync offline data to server when device is back online


### models

Contains the `model classes` required for the app

### repositories

This directory contains classes required to get the data required for the app using helper classes

### Utils

Contains the `common file(s)`, `app routes` and `utilities` used in the project.

### view_models

Contains the `view models` for the views, which helps in having business logics separately

### Widgets

Contains the `UI components` like common widgets and various other screens.


``` 
widgets/ 
|- common_widgets/ 
. 
. 
. 
```


### main.dart

This is the `starting point` of the application. All the application level configurations are defined in this file