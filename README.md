### reproduce steps

`yarn`

check if dev mode working

`yarn dev` stop by ctrl+c

`yarn build`

check if prod mode working

`yarn start` stop by ctrl+c

build binary by pkg and run it

`yarn run pkg`

`yarn run pkg` execute `pkg --targets node8-macos-x64 server.js --out-path pkg && NODE_ENV=production ./pkg/server` , might change `--targets` to `node8-linux-x64` or `node8-win-x64` for your OS.

```
pkg --targets node8-macos-x64 server.js --out-path pkg && NODE_ENV=production ./pkg/server
> pkg@4.3.7
/snapshot/youtube-collector-app/node_modules/next-server/dist/server/next-server.js:303
                throw new Error(`Could not find a valid build in the '${this.distDir}' directory! Try
building your app with 'next build' before starting the server.`);
```
