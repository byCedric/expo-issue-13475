# Issue 13475

This repository demonstrates the different behavior on Windows from [issue 13475](https://github.com/expo/expo/issues/13475).

> This issue [has been fixed in `@unimodules/react-native-adapter@6.3.2`](https://github.com/expo/expo/pull/13494).

## Steps

- Setup the repository, node (14), and Expo CLI.
- Create a new bare project using SDK 42
- Add a resolution to change the library
- Build a debug APK

## Tests

The workflows in this repository are executed on different operating systems, using versions:

- `@unimodules/react-native-adapter@6.3.1` as "before fix"
- `@unimodules/react-native-adapter@6.3.2` as "after fix"

### Results

| OS      | Before fix                                                                             | After fix                                                                              |
| ------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| windows | [_❌ failure_](https://github.com/byCedric/expo-issue-13475/actions/runs/1005486985)   | [**✅ success**](https://github.com/byCedric/expo-issue-13475/actions/runs/1005487764) |
| macos   | [**✅ success**](https://github.com/byCedric/expo-issue-13475/actions/runs/1005487190) | [**✅ success**](https://github.com/byCedric/expo-issue-13475/actions/runs/1005487952) |
| ubuntu  | [**✅ success**](https://github.com/byCedric/expo-issue-13475/actions/runs/1005487424) | [**✅ success**](https://github.com/byCedric/expo-issue-13475/actions/runs/1005488183) |
