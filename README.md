# Algola Vue Module Not Found Warning Repro

> This repo reproduces the warning referenced in this issue: https://github.com/algolia/vue-instantsearch/issues/818

## Steps taken to setup this repo

1. Setup basic Laravel Mix [according to the docs](https://laravel-mix.com/docs/5.0/installation).
2. Install Algolia's Vue Instant search [according to the docs](https://www.algolia.com/doc/guides/building-search-ui/getting-started/vue/#initialization)
3. Watch or build results in the following warning:
   - `yarn build`

```
 WARNING  Compiled with 1 warnings                                                          3:16:58 PM

 warning  in ./node_modules/vue-instantsearch/dist/vue-instantsearch.esm.js

Module not found: Error: Can't resolve 'vue-server-renderer/basic' in '/Users/saltymouse/webdev/my-app/node_modules/vue-instantsearch/dist'

           Asset       Size     Chunks             Chunk Names
    /dist/app.js    1.1 MiB  /dist/app  [emitted]  /dist/app
/dist/index.html  258 bytes             [emitted]
    dist/app.css   42 bytes  /dist/app  [emitted]  /dist/app

WARNING in ./node_modules/vue-instantsearch/dist/vue-instantsearch.esm.js
Module not found: Error: Can't resolve 'vue-server-renderer/basic' in '/Users/saltymouse/webdev/my-app/node_modules/vue-instantsearch/dist'
 @ ./node_modules/vue-instantsearch/dist/vue-instantsearch.esm.js
 @ ./src/app.js
 @ multi ./src/app.js ./src/app.scss
✨  Done in 2.76s.
```
