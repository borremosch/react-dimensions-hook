# react-dimensions-hook

This package allows you to measure the size of any HTML element inside one of your React functional components using hooks.

## Usage

```tsx
import { useDimensions } from 'react-dimensions-hook';

function MyComponent() {
  const { ref, dimensions } = useDimensions();

  return (
    <div
      ref={ref}
      style={{
        width: '500px',
        height: '100px',
        margin: '0 auto'
      }}
    >
      my size is {dimensions.width} × {dimensions.height}
    </div>
  );
}
```

## Features

- Uses react hooks
- TypeScript compatible
- Uses [react-observer-polyfill](https://www.npmjs.com/package/resize-observer-polyfill) to detect all changes in size

## Attribution

While this package was written from scratch, inspiration was gained from [react-dimensions](https://www.npmjs.com/package/react-dimensions), [react-sizeme](https://www.npmjs.com/package/react-sizeme), and [react-use-dimensions](https://www.npmjs.com/package/react-use-dimensions)
