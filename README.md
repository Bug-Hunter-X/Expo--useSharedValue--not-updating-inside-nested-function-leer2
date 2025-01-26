# Expo `useSharedValue` Hook Issue

This repository demonstrates a bug where the Expo `useSharedValue` hook does not update correctly when used within a nested function. The shared value remains unchanged despite attempts to modify it.  The issue is detailed below.

## Problem Description
The problem arises when trying to update a `useSharedValue` from within a function called by an event handler (e.g., a button press).  The shared value's state does not reflect the change.

## Solution
The solution involves using `callback` to update the value.