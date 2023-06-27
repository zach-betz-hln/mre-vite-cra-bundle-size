# Minimal, Reproducible Example for CRA vs Vite Bundle Size

Make sure to compare the **gzip** values.

For each SPA tool, re-run this to gather bundle size:

```
rm -rf dist build ; npm run build
```

## When First Created

CRA:

```
File sizes after gzip:

46.62 kB  build/static/js/main.9391c6f4.js
1.78 kB   build/static/js/787.93ab6bb5.chunk.js
```

Vite:

```
dist/assets/index-c7e05d32.js   143.41 kB │ gzip: 46.10 kB
```

## With Apollo Client

Installed with:

```
npm install "@apollo/client"
```

CRA:

```
File sizes after gzip:

89.06 kB  build/static/js/main.a4e68eb0.js
1.78 kB   build/static/js/787.93ab6bb5.chunk.js
```

Vite:

```
dist/assets/index-91592e7f.js   289.37 kB │ gzip: 89.91 kB
```
