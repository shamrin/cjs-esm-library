# Universal CommonJS / ESM / TypeScript library example

Build `test-lib.cjs` (CommonJS) and `test-lib.js` (ESM) in one go:

```
npm run build
```

Develop library in the browser, with hot reload:

```
npm run dev
```

Try the library in Node:

```
$ node
> const {hello} = await import('./dist/test-lib.cjs')
undefined
> hello()
hello world
```

## Details

This example was build by following Vite guide:

```
npm create vite@latest test-lib -- --template vanilla-ts
```

And then by adding ["Library Mode"] config, with few small tweaks. 

["Library Mode"]: https://vitejs.dev/guide/build.html#library-mode
