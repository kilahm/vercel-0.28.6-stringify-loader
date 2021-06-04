Reproduction steps

In one terminal window:

```sh
npm i
npm run build
```

In a separate terminal window:

```sh
echo "console.log('bar');" > index.ts
```

In the first terminal window observe output similar to:

```sh
ncc: Version 0.28.6
ncc: Compiling file index.js
File change, rebuilding...
ncc: Using typescript@4.3.2 (local user-provided)
 0kB  dist/index.js
40kB  dist/sourcemap-register.js
 0kB  dist/index.js.map
40kB  [1233ms] - ncc 0.28.6
Watching for changes...
File change, rebuilding...
ModuleNotFoundError: Module not found: Error: Can't resolve '/ncc-bug/node_modules/@vercel/ncc/dist/ncc/loaders/stringify-loader.js' in '/ncc-bug'
Watching for changes...
```


