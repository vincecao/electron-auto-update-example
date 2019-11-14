# Electron Auto Update Example

# Add token with your git
- Go for Github [token page](https://github.com/settings/tokens/new)
- (option)Add in environment 
``` bash
# macOS/linux:
export GH_TOKEN="<YOUR_TOKEN_HERE>"

# Windows with powershell:
[Environment]::SetEnvironmentVariable("GH_TOKEN","<YOUR_TOKEN_HERE>","User")
```
- Add `repo `
- Modify _package.json_
```
"appId": "com.example.ElectronAutoUpdate",
"publish": [{
  "provider": "github",
  "owner": <YOUR-NAME>,
  "repo": "electron-auto-update-example",
  "token": <YOUR-TOKEN>
}]
```

# Deploy
run `npm run deploy`
_For Mac need Developer Account_

# Test
Download the old [release](https://github.com/vincecao/electron-auto-update-example/releases) (v 1.0.2), it will auto download new and restart

# Reference
-  Original fork from [electron-auto-update-example](https://github.com/johndyer24/electron-auto-update-example), [this medium article](https://medium.com/@johndyer24/creating-and-deploying-an-auto-updating-electron-app-for-mac-and-windows-using-electron-builder-6a3982c0cee6)
- [electron-updater-example](https://github.com/iffy/electron-updater-example)
