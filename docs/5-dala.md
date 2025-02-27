# U2A - Documentation | Deleting a local app


> [!WARNING] Make sure that the app is closed before removing it.

Wanna get rid of an app ? Sure ! Simply do:
```bash
u2a remove <appname>
```
<h6>'appname' is either the domain of the app or the name you set with `--name`</h6>

It will automaticly remove your app.

Example:
```shell
PS C:\Users\douxx> u2a remove "Claude AI"
? Are you sure you want to remove the application for Claude AI? Yes
[12:38:33 PM] - SUCCESS | Shortcut removed from the Start Menu: C:\Users\douxx\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\U2A Apps\Claude AI.lnk
[12:38:34 PM] - INFO | Removing the application Claude AI...
[12:38:34 PM] - SUCCESS | The application for Claude AI has been successfully removed
```
