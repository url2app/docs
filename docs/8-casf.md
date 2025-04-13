# U2A - Documentation | Creating a setup file

> [!WARNING] Setup files creation might not work as excepted on MacOs and Linux.

U2A can also create an installer for your webapp, so people can install it on their system easily.

To create a setup file add the parameter `--setup` to the existing [executable command](?p=create-executable) to get something like this:

```bash
u2a create <url/domain> --executable --setup
```

This will create a directory in your [working directory](https://en.wikipedia.org/wiki/Working_directory) containing the executable, and one containing the setup. (You dont need to provide the directory containing the executable to run the setup).

Example with [Youtube.com](https://youtube.com):

```shell
PS C:\Users\douxx\etc>  u2a create youtube.com --name "Youtube" --executable --setup
[01:07:54 PM] - INFO | Creating application for youtube.com
[01:07:54 PM] - INFO | Getting the icon path for https://youtube.com
[01:07:54 PM] - SUCCESS | Site icon downloaded and saved for youtube.com
[01:07:54 PM] - WARN | To proceed to setup, favicon has been resized to 256x256. Quality loss is possible.
[01:07:54 PM] - INFO | Installing dependencies for Youtube
[01:08:01 PM] - INFO | Building executable for win32...
[01:08:10 PM] - INFO | Building setup for win32...
[01:08:30 PM] - SUCCESS | Setup installer created at: C:\Users\douxx\etc\Youtube-setup
[01:08:30 PM] - SUCCESS | Executable created at: C:\Users\douxx\etc\Youtube-executable
```

As we can see, the `Youtube-setup` Folder contains the youtube setup files. You need to provide all of them to get the setup to work.

![Setup files](assets/img/setup1.png)