# U2A - Documentation | Creating an executable

> [!WARNING] Executables creation might not work as excepted on MacOs.

U2A also supports executables files (like .exe) creation, so you can easily share a webapp without installing it or downloading U2A on all machines.

To do so, add to the [create command](?p=create-local-apps) an `--executable` parameter.
You can also specify the target system next to the paramter (`--executable [windows|darwin|linux]`) | If not specified it will take the host system.

- Windows: `win32`
- Darwin: `MacOs`
- Linux: `Linux`

And the architecture with `--arch [x64|armv7l|arm64|universal]` | If not specified it will take the host architecture.

> [!WARNING] `universal` is meant for apple specific architecture, not for all architectures

The command will then create a directory in your [working directory](https://en.wikipedia.org/wiki/Working_directory) containing the executable.
No local application will be installed when you create an executable.

> [!INFO] Other parameters like `--name` also work on executables

Example with [Youtube.com](https://youtube.com):
```shell
PS C:\Users\douxx\etc>  u2a create youtube.com --name "Youtube" --executable
[12:56:42 PM] - INFO | Creating application for youtube.com
[12:56:43 PM] - INFO | Getting the icon path for https://youtube.com
[12:56:43 PM] - SUCCESS | Site icon downloaded and saved for youtube.com
[12:56:43 PM] - INFO | Installing dependencies for Youtube
[12:56:51 PM] - INFO | Building executable for win32...
[12:56:58 PM] - SUCCESS | Executable created at: C:\Users\douxx\etc\Youtube-executable
```
