# HTTP way of using Electron-Updater example

## Deploy
- Drag package.json into root path
- Build command, `npm run build` (windows user can not build for mac version)
- Copy all `dist` files into `wwwroot` folder, look for wwwroot example
``` bash
mkdir -p wwwroot
cp dist/* wwwroot/
```
- Run the local server in test, `node_modules/.bin/http-server wwwroot/ -p 8080`
