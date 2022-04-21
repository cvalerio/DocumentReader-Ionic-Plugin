# How to build demo application
1. Visit [licensing.regulaforensics.com](https://licensing.regulaforensics.com) to get a trial license (`regula.license` file). The license creation wizard will guide you through the necessary steps.
2. Download or clone this repository using the command `git clone https://github.com/regulaforensics/DocumentReader-Ionic-Plugin.git`.
3. Run the following commands in Terminal:
```bash
$ cd example
$ npm install
$ npx jetify
$ ionic cordova prepare
```
4. Copy the `regula.license` file to the `example/src/assets` folder.

5. Android:
  * Run `ionic cordova build android`, then`ionic cordova run android` inside `example` folder - this is just one way to run the app. You can also run it directly from within Android Studio.

6. iOS:
  * Run `ionic cordova build ios`, then `ionic cordova run ios` inside `example` folder - this is just one way to run the app. You can also run it directly from within Xcode.


# Troubleshooting license issues
If you have issues with license verification when running the application, please verify that next is true:
1. The OS, which you use, is specified in the license (e.g., Android and/or iOS).
3. The license is valid (not expired).
4. The date and time on the device, where you run the application, are valid.
5. You use the latest release version of the Document Reader SDK.
6. You placed the `license` into the correct folder as described [here](#how-to-build-demo-application).
