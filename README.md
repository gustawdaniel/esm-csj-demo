# Demo of npm package with ESM and CJS build

Install by

```json
    "sumesm": "file:./../esm"
```

in project next to this directory and use this import:

```typescript
const s = require('sumesm');

console.log(s.sum(1, 2));

(async () => {
    const s = await import('sumesm');
    console.log(s.sum(1, 2));
})()
```

Blog post:

https://preciselab.io/simplest-tutorial-for-esm-commonjs-package-creators/
