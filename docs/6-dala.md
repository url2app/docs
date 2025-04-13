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
[12:01:43 AM] - INFO | Removing the application Claude AI...
[12:01:43 AM] - SUCCESS | Shortcut removed from the Start Menu: C:\Users\douxx\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\U2A Apps\Claude AI.lnk
[12:01:43 AM] - SUCCESS | Icon for Claude AI removed
[12:01:44 AM] - SUCCESS | Application data folder removed: C:\Users\douxx\AppData\Roaming\u2a-Claude-AI
[12:01:44 AM] - SUCCESS | Application files removed: C:\Users\douxx\.u2a\apps\Claude AI
[12:01:44 AM] - SUCCESS | The application for Claude AI has been successfully removed
```
