# React 18+ useEffect Warning: Missing Cleanup in setInterval
This repository demonstrates a common error in React 18 and above: forgetting to include a cleanup function in a useEffect hook that uses setInterval. This can lead to memory leaks and unexpected behavior.

## Bug
The `bug.js` file contains a component that uses setInterval within a useEffect hook without a cleanup function. This will trigger a warning in React 18+.

## Solution
The `bugSolution.js` file shows the corrected code with the cleanup function added using `clearInterval`. This prevents memory leaks and ensures that the interval is stopped when the component unmounts.