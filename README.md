# Google Cloud Storage TypeScript reproduction

This example reproduces a TypeScript declaration error in `@google-cloud/storage` 9.0.0.

Use Node.js 22 or later:

```sh
npm ci
npm run build
```

The build reports:

```text
node_modules/@google-cloud/storage/build/esm/src/file.d.ts(1069,50): error TS2552: Cannot find name 'CreateWriteStreamOptionsInternal'. Did you mean 'CreateWriteStreamOptions'?
```

The error occurs before any Cloud Storage API request is made.
