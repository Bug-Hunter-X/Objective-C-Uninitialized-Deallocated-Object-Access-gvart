# Objective-C Uninitialized/Deallocated Object Access

This repository demonstrates a common Objective-C error: accessing uninitialized or deallocated objects. This can lead to crashes or unpredictable behavior.  The example code shows several problematic scenarios and how to fix them using proper initialization and memory management techniques.

## Problem

In Objective-C, you can run into issues if you try to use an object's properties before it's been fully initialized or after it's been deallocated.  This often leads to crashes or unexpected program behavior (sometimes subtle).

## Solution

The solutions mainly focus on:

* **Proper initialization:** Ensure all object properties are correctly set in the designated initializer (`init` or `initWith...`).
* **Memory management:** Use ARC or manual retain/release effectively to prevent premature deallocation.
* **Nil checking:**  Always check for `nil` before accessing an object's properties.