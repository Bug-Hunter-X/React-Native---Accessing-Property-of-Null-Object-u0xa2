# React Native - Accessing Property of Null Object

This repository demonstrates a common error in React Native: attempting to access a property of a null or undefined object.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides a solution using optional chaining and nullish coalescing.

## Problem

Accessing object properties before checking for null or undefined values can lead to runtime errors.  This often occurs when dealing with asynchronous data fetching or when state isn't properly initialized.

## Solution

The solution involves employing optional chaining (`?.`) and the nullish coalescing operator (`??`) to safely access properties.  Optional chaining short-circuits the expression if the object is null or undefined, preventing the error.  The nullish coalescing operator provides a default value if the property is null or undefined.