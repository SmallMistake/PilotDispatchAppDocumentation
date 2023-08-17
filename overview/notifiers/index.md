# Notifiers

<blockquote>
<strong>Summary</strong>: Notify scripts of data change from anywhere in the app with notifiers.
</blockquote>

## Overview
Notifiers are special classes that sit above the rest of the flutter tree. Whenever you want to get or listen to data you can call a Provider to get you a reference to a notifier. Using that reference you can use the values on the notifier to update your app across the board.

Documentation: [ChangeNotifier API Link](https://api.flutter.dev/flutter/foundation/ChangeNotifier-class.html)

## Using a Notifier
When ever you need to get data from a provider you will need to get a reference to it from a provider. It is common to put these in the build functions of widgets.
<blockquote>
var preferencesNotifier = Provider.of<PreferencesNotifier>(context);
</blockquote>

## Extending a Notifier
You will usually want to extend a ChangeNotifier so that you can track your own values.

Steps:
1) Extend the ChangeNotifier
2) Add a functions and variables you want to track
3) Add an initializer in the main.dart file

<blockquote>
<pre>
<strong>Class Example</strong>
class PreferencesNotifier with ChangeNotifier {
  double textScaleFactor = 1.0;
  bool allowPageScrolling = false;

  PreferencesNotifier();

  double get iconsSize => textScaleFactor * 17;

  Future<void> initialize() async {
    var prefs = await SharedPreferences.getInstance();
    textScaleFactor = prefs.getDouble('textScaleFactor') ?? 1.0;
  }

  setTextScaleFactor(double x) {
    textScaleFactor = x;
    notifyListeners();

    SharedPreferences.getInstance().then(
      (prefs) {
        prefs.setDouble('textScaleFactor', textScaleFactor);
      },
    );
  }

  void restoreSettings() {
    textScaleFactor = 1.0;
    notifyListeners();
  }
}

<strong>Initialization Example</strong>
(In main.dart file)
Future<void> main() async {
    ...
    final preferencesNotifier = PreferencesNotifier();
    await preferencesNotifier.initialize();
    ...
}
</pre>
</blockquote>