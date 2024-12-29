# Unclear Expo CLI Android Build Errors

This repository demonstrates a common yet frustrating issue encountered when building Android APKs using the Expo CLI. The error messages are often vague, making debugging difficult.  This example focuses on issues arising from incorrect Android SDK configurations, Gradle problems, or dependency conflicts, particularly with libraries that manage splash screens.

## Problem

The Expo CLI build process fails with unhelpful error messages.  The specific message varies, but generally indicates problems within the Android build system or Gradle.

## Solution

The solution involves verifying the Android SDK setup, resolving Gradle issues (by cleaning and rebuilding, or updating Gradle), and carefully managing dependencies, especially those that might conflict with Expo's built-in functionality (like splash screens). Removing conflicting libraries or using Expo's built-in features is often the best approach.

## How to Reproduce

1. Clone this repository.
2. Follow the instructions in `bug.js` to see an example of a problematic setup (commented out by default).
3. Try building the Android APK using the Expo CLI. Observe the error.
4. Uncomment the problematic code or add a conflicting library and retry.
5. Then, use `bugSolution.js` to implement the solution and retry the build process. 