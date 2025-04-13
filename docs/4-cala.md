# U2A - Documentation | Creating a local app

Once you [installed UrlToApp](?p=installation), you will be able to install 'websites' as apps locally. We will see how on this page.

### Basic install
To create an application quickly, simply run the command
```bash
u2a create <url/domain>
```

Let's try with [Claude.ai](https://claude.ai):
```shell
PS C:\Users\douxx> u2a create claude.ai
[11:37:58 AM] - INFO | Creating application for claude.ai
[11:37:58 AM] - INFO | Getting the icon path for https://claude.ai
[11:37:58 AM] - SUCCESS | Site icon downloaded and saved for claude.ai
[11:37:58 AM] - INFO | Installing dependencies for claude.ai
[11:38:01 AM] - SUCCESS | Shortcut created in the Start Menu: C:\Users\douxx\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\U2A Apps\claude.ai.lnk
[11:38:01 AM] - SUCCESS | Application successfully created for https://claude.ai
[11:38:01 AM] - INFO | A shortcut has been created in your system's applications directory
```

As we can see, Claude's app has been created and is runnable on our system:
![Claude app](assets/img/claude1.png)

### Personalized install
U2A allows you to personalize your installation, with those command parameters:
`--name <name>`: Set the name of the app (eg `Claude` instead of `claude.ai`)  
`--witdh <int>`: Set the witdh of the app window that will be created. (Default `1200`)  
`--height <int>`: Set the height of the app window that will be created. (Default `800`)
`--icon <path>`: Use a custom .ico file instead of the default / fetched one

Let's try to personalize [Claude.ai](https://claude.ai):

```shell
PS C:\Users\douxx> u2a create claude.ai --name "Claude AI" --width 600 --height 400
[12:13:01 PM] - INFO | Creating application for claude.ai
[12:13:02 PM] - INFO | Getting the icon path for https://claude.ai
[12:13:02 PM] - SUCCESS | Site icon downloaded and saved for claude.ai
[12:13:02 PM] - INFO | Installing dependencies for Claude AI
[12:13:06 PM] - SUCCESS | Shortcut created in the Start Menu: C:\Users\douxx\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\U2A Apps\Claude AI.lnk
[12:13:06 PM] - SUCCESS | Application successfully created for https://claude.ai
[12:13:06 PM] - INFO | A shortcut has been created in your system's applications directory
```

As we can see, the app is now named "Claude AI" and the windows is 600x400
![Claude app](assets/img/claude2.png)
![Claude app](assets/img/claude3.png)