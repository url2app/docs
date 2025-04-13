# U2A Technical details & Troubleshooting | File structure

Here we will see how u2a files are structured, and where they are placed on your operating system.

> [!INFO] `~` will represent the user home, `\Windows\Users\user` on Windows and `/home/user` on MacOs and Linux

### Applications and logs
U2A stores all the content of local webapps and logs files into the `~/.u2a` folder.

`~/.u2a` content:

```shell
├── apps/
├── db.json
├── logs/
├── postinstall.json
└── settings.json
```

`apps` contains all favicons and webapps datas.
`logs` contains all the logs for the create, list, remove and favicon features.
`db.json` contains all the datas of currently installed applications
`postinstall.json` is for the postinstall script, dont touch it please, or `settings.json` will be resetted
`settings.json` contains different settings, configurable with the `configure` command

### Menu/Launcher files
To insert an application into the menu/launcher of your os, U2A must create some specific files on your os.

**Windows**: U2A stores shortcuts into `~\AppData\Roaming\Microsoft\Windows\Start Menu/Programs\U2A Apps\`
**Linux**: U2A stores desktop entries into `~/.local/share/applications/`
**MacOs**: U2A stores applications into `~/Applications/U2A Apps/`

### Application files
U2A has a specific folder to store application files, like local storage or cache.

> [!NOTE] In versions `<=3.4.2`, those files aren't automaticly deleted by u2a. You have to remove them manually if you want them off.

**Windows**: Files are stored into `~\AppData\Roaming\u2a-*\`
**Linux**: Files are stored into `~/.config/u2a-*/`
**Windows**: Files are stored into `~/Library/Application Support/u2a-*/`
