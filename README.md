# CS 442 – Week 1 Lab Task

## Enhance the Counter App

**Student Name:** Hamza A  
**Roll Number:** 04072313001  
**Course:** CS 442 – Mobile Application Development  
**Lab:** Week 1 Lab Task

## Personal Parameters

- **myThreshold:** 6
- **mySeedColor:** `Colors.amber`

### Threshold Calculation

Last 3 digits of roll number:

`001`

Sum:

`0 + 0 + 1 = 1`

Then add 5:

`1 + 5 = 6`

Therefore:

```dart
const int myThreshold = 6;
const Color mySeedColor = Colors.amber;
```

## Tasks Completed

### 1. Reset Button
Added a second Floating Action Button with `Icons.refresh`. When pressed, the counter resets to 0.

### 2. Personalised Threshold Message
The message **"You're on a roll!"** appears in green only when the counter is greater than `myThreshold`.

### 3. Reset Counter Tracker
Added a separate state variable to track how many times the Reset button has been pressed. The screen displays:

```text
Resets used: N
```

### 4. Personalised Theme
The application theme uses:

```dart
colorSchemeSeed: mySeedColor
```

with `Colors.amber`.

### 5. About Line
The application displays:

```text
Built by Hamza A · 04072313001
```

## Screenshot

Add a screenshot of the running application below. The screenshot should show:
- Counter above the threshold
- **"You're on a roll!"** message visible
- At least one reset performed
- `Resets used: 1` (or a higher number)

Save your screenshot in the repository, for example as:

```text
screenshot.png
```

Then add it here:

```markdown
![Running App Screenshot](image.png)
```

## Written Reflection

`setState(() {...})` tells Flutter that the state of a StatefulWidget has changed and that the screen should be rebuilt using the new values. In this app, when the counter or reset count changes, `setState()` makes those new values appear on the screen. Without calling `setState()`, changing the state variable alone does not tell Flutter to rebuild the widget, so the updated value may not be displayed.

## Testing

The application was tested by:
- Increasing the counter using the `+` button.
- Checking that **"You're on a roll!"** appears when the counter becomes greater than 6.
- Pressing the refresh button to reset the counter to 0.
- Checking that the reset counter increases after each reset.
- Checking that the two Floating Action Buttons do not overlap.

## Submission

This repository contains the Flutter project and the completed `lib/main.dart` for the CS 442 Week 1 Lab Task.
