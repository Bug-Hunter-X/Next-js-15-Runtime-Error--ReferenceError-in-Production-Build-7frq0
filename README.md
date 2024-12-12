# Next.js 15 Runtime Error: ReferenceError in Production Build

This repository demonstrates a runtime error in a Next.js 15 application that occurs only in the production build. The error is caused by referencing an undeclared variable within a page component.

## Bug

The `pages/about.js` file attempts to access a variable (`nonExistentVariable`) that is not defined, leading to a `ReferenceError` at runtime. This error is not detected during development because Next.js's development environment might have different variable scopes or configurations.

## Solution

The solution is to ensure that all variables are properly declared and initialized before use. The corrected `pages/aboutSolution.js` demonstrates proper variable declaration.  The use of TypeScript would also help avoid these errors.