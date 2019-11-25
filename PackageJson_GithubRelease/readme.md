# Github release page for Electron-Updater example

Go to github release page for exe downloads

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
"publish": [
      {
        "provider": "github",
        "owner": "<YOUR-USER-NAME>",
        "repo": "electron-auto-update-example",
        "token": "<YOUR-TOKEN>"
      }
    ]
```

## Deploy
- Drag package.json into root path
- Build command, `npm run depoly` (windows user can not build for mac version)
- Need manual comfirm publish button.

_For Mac need Developer Account_

# Test
Download the old [release](https://github.com/vincecao/electron-auto-update-example/releases) (v 1.0.2), it will auto download new and restart
