# Expo Linking API Inconsistency on Android

This repository demonstrates a bug related to the Expo `Linking` API's inconsistent behavior on Android devices. The issue involves unreliable triggering of `Linking.addEventListener`, leading to unpredictable deep link handling.  The inconsistency is amplified by specific Android versions and potentially configurations.

## Bug Description
The `Linking.addEventListener` function, crucial for managing incoming URLs from deep links, does not consistently trigger on Android. This may cause the application to fail to respond to deep links, resulting in a poor user experience.

## How to Reproduce
1. Clone this repository.
2. Install dependencies: `npm install`
3. Run the app on an Android emulator or device.
4. Attempt to open a deep link associated with the app.  Observe that the deep link may or may not be handled correctly, demonstrating the inconsistent behavior.  (Specific details on reliable reproduction may depend on the Android version).

## Solution
The solution involves implementing a more robust approach to deep link handling, possibly using alternative methods or incorporating error handling and fallback mechanisms.