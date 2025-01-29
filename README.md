# Firebase onAuthStateChanged Unsubscribe Issue

This repository demonstrates a common issue when using Firebase's `onAuthStateChanged` listener: improper unsubscription.  Leaving listeners active after a component unmounts leads to memory leaks and can cause unexpected behavior in your application.

The `bug.js` file shows the incorrect implementation where the unsubscribe function isn't properly handled. The `bugSolution.js` provides a corrected version with a proper cleanup function to prevent these issues.  This ensures that the listener is detached when it's no longer needed.