# Checking your Setup

It can be difficult to know if you've followed all the steps correctly. There
are so many things that can go wrong, and everyone's computer is different. To
help with this problem, here is a script that checks your setup
to verify it is done correctly.

To run this script, simply open a terminal and run this command:

```shell
curl -s https://raw.githubusercontent.com/C9DevLegends/setup-checker/master/run.sh | bash
```

This command will download a script from our github page and if your setup is correct
you should see an output like this:
```shell
Checking macOS

―――――――――――――――――――――
macOS Version: 13.0
―――――――――――――――――――――

Checking Shell

―――――――――――――――――――――
Shell: zsh
Shell Startup File: ~/.zshrc
―――――――――――――――――――――

Checking Node.JS

―――――――――――――――――――――
Node Binary: /Users/echo/.nvm/versions/node/v18.1.0/bin/node
Node Version: v18.1.0
NPM Binary: /Users/echo/.nvm/versions/node/v18.1.0/bin/npm
NPM Version: 8.3.1
Mocha Binary: /Users/echo/.nvm/versions/node/v18.1.0/bin/mocha
Mocha Version: 9.2.2
―――――――――――――――――――――

Checking VSCode

―――――――――――――――――――――
Code Binary: /usr/local/bin/code
Version: 1.77.0
―――――――――――――――――――――

Checking Python

―――――――――――――――――――――
pyenv version: pyenv 3.10.2
Python Binary: /Users/echo/.pyenv/shims/python
Python3 Binary: /Users/echo/.pyenv/shims/python3
Python Version: 3.10.2
Pipenv Binary: /Users/echo/.pyenv/shims/pipenv
Pipenv Version: pipenv, version 2023.10.24
―――――――――――――――――――――

Checking Docker

―――――――――――――――――――――
Docker Binary: /usr/local/bin/docker
Docker Version: Docker version 20.10.13, build 5056854
―――――――――――――――――――――

Congratulations! All software is up to date!

―――――――――――――――――――――
```

If you get the Congratulations message you'll know you have everything setup
properly. The script tries to tell you what steps you should probably take
if some piece fails.

If you get a failure and don't know how to fix it, feel free to post your output
in Slack or to ask a teammate for help.
