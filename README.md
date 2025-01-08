# Expo CLI Error: Unsupported Module Import

This repository demonstrates a common but often overlooked error in Expo CLI projects: attempting to import modules that are not supported within Expo's managed workflow.  This usually manifests as an error during build or runtime.

## The Problem

Expo, while convenient, restricts access to certain Node.js modules for security and maintainability reasons.  Attempting to import these modules (e.g., `crypto`, modules relying on native code without Expo equivalents) directly leads to errors.

## Solution

The solution depends on the module in question.  Sometimes Expo provides alternative modules; other times, you may need to eject from the managed workflow to a bare React Native project for complete control.