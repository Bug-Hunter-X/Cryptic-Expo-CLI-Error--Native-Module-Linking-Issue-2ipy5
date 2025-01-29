# Expo CLI: Cryptic Native Module Linking Error

This repository demonstrates a common yet difficult-to-diagnose error in Expo CLI projects involving native module linking.  The error message is often unhelpful, making debugging challenging.

## Problem

The core problem is a mismatch between native modules required by your Expo app and those available on your device/simulator. This frequently occurs after updates (Expo, native dependencies), or project structure changes affecting the linking process.

The resulting error message can be very cryptic, offering little insight into the root cause.  This repo provides an example of such a situation and how to approach the debugging and resolution process.

## Solution

The solution involves carefully examining your package.json and potentially your Podfile (iOS) or build.gradle (Android) to ensure all native dependencies are correctly installed, configured, and linked.  Specific strategies are included in the solution file.

## How to reproduce

1. Clone the repo.
2. Follow instructions in `expoBug.js` to reproduce the cryptic error.
3. Compare the steps in `expoBug.js` with the solution in `expoBugSolution.js` to understand the debugging process.