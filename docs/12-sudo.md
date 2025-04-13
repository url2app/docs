# U2A Technical details & Troubleshooting | Running as root

Since version `3.3.0`, U2A automaticly rejects commands being run as administrator for obvious security reasons.
But, if you are sure of what you are doing, you can add a `--allowroot` option to your command, and it will be accepted

> [!DANGER] Running an app as administrator can cause serious issues. Be sure of what you're doing!