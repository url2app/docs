# U2A Technical details & Troubleshooting | File structure

Here we will see how u2a files are structured, and where they are placed on your operating system.

> [!INFO] `~` will represent the user home, `\Windows\Users\user` on Windows and `/home/user` on MacOs and Linux

### Applications and logs
U2A stores all the content of local webapps and logs files into the `~/.u2a` folder.

`~/.u2a` content:

```shell
├── apps/
├── db.json
└── logs/
```

`apps` contains all favicons and webapps datas.
`logs` contains all the logs for the create, list, remove and favicon features.
`db.json` contains all the datas of currently installed applications

### Menu/Launcher files
To insert an application into the menu/launcher of your os, U2A must create some specific files on your os.

**Windows**: U2A stores shortcuts into `~\AppData\Microsoft\Windows\Start Menu/Programs\U2A Apps\`
**Linux**: U2A stores desktop entries into `~/.local/share/applications/`
**MacO**: U2A stores applications into `~/Applications/U2A Apps/`