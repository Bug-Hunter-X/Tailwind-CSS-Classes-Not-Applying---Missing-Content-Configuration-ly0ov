# Tailwind CSS Classes Not Applying - Missing Content Configuration

This repository demonstrates a common issue when using Tailwind CSS: classes not being applied due to a missing or incorrectly configured `content` array in `tailwind.config.js`.

## Bug Description
Tailwind CSS classes are included in the HTML, but they have no visual effect. The issue stems from an absence or incorrect specification of the source files in the `content` array within `tailwind.config.js`.  This prevents Tailwind from correctly identifying and processing the classes used in your project.

## How to Reproduce
1. Clone this repository.
2. Install the dependencies: `npm install`
3. Run the project and observe that the Tailwind classes are not applied (in `bug.js`).
4. Observe the fix in the `bugSolution.js` file.

## Solution
Ensure that the `content` array in your `tailwind.config.js` correctly points to the files containing the Tailwind CSS classes. This allows Tailwind to correctly process and apply the styles.

## Key takeaway
Always verify your `content` array in your `tailwind.config.js`. Using `purge` is deprecated, use `content` instead.