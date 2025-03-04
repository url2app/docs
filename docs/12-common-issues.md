# U2A Technical details & Troubleshooting | Common issues

Here we will list some common issues and give possible solutions.

### 1. U2A isn't launching
> Make sure that you correctly installed U2A, if so, try reinstalling it.

### 2. Error ERR_REQUIRE_ESM while launching
> This error occures when you are launching U2A with a version of node under 22.0.0. Update your node installation to avoid this error

### 3. Other error while launching
> Errors can occurs when launching u2a. When it happen without being mentionned in the documentation, please [create an issue on github](https://github.com/url2app/urltoapp/issues). To try to bypass the error, you can still try to clone the github repository, navigate into it, run the commande `npm i` and then `npm start` instead of `u2a`.

### 4. U2A isn't creating my app
> Make sure you gave the program the correct permissions. If you are on MacOs or linux try running it with `sudo`.

### 5. U2A isn't removing my local webapp
> Make sure that you don't have the application opened. If you are on MacOs or linux try running it with `sudo`.

### 6. U2A isn't loading the icon of my website
> To retrive the icon, U2A uses favicons, so you need to have a favicon.ico file at the root of your website so U2A can fetch it.

### 7. U2A isn't giving me an executable / setup file
> Try [troubleshooting the issue](?p=troubleshooting) with the log files or debug mode.

> [!NOTE] If you need further help, [create an issue on github](https://github.com/url2app/urltoapp/issues) or send an email to [contact@urltoapp.xyz](mailto:contact@urltoapp.xyz)