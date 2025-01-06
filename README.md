# Next.js 15: Missing Default Export in Page Component

This repository demonstrates a common error encountered in Next.js 15: forgetting to export a default function from a page component.  Even a simple functional component needs to be exported as default for Next.js to recognize it as a valid page.

## Bug Description

If a page component does not have a default export, Next.js 15 will throw an error, preventing the page from rendering correctly.  This is a subtle error that can be difficult to debug.

## Reproduction

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Navigate to `/about`. You'll encounter a Next.js error.

## Solution

The solution is simple: ensure that your page component exports a default function.  See `aboutSolution.js` for a corrected example.

## Additional Notes

This issue is particularly relevant in larger projects where components might be easily overlooked.  Careful attention to the export statement is crucial when building Next.js applications.
