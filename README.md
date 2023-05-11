# Flutter Battery Plus

A Flutter plugin to access various information about the battery of the device the app is running on.

## Usage

Add battery_plus as a dependency in your pubspec.yaml file.

## Example

   ```
   // Import package
import 'package:battery_plus/battery_plus.dart';

// Instantiate it
var battery = Battery();

// Access current battery level
print(await battery.batteryLevel);

// Be informed when the state (full, charging, discharging) changes
battery.onBatteryStateChanged.listen((BatteryState state) {
  // Do something with new state
});
   ```
