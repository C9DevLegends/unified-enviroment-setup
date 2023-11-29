# Installing Node.JS

Node.JS, a JavaScript Runtime Environment, facilitates the direct execution of JavaScript files on a computer. Although JavaScript is integrated into every web browser, if you wish to run JavaScript without a browser, you need to install Node.JS.

> **NOTE:** We abstain from using the installer provided at the Node.JS website. If you already have it installed, please uninstall it before proceeding with these instructions.

## Node Version Manager (nvm)

As a developer, you often juggle multiple projects on your computer, each requiring a different Node.JS version. Installing a new version directly from the Node.JS website can be challenging and error-prone. Fortunately, Node Version Manager, or `nvm`, is an open-source tool designed to assist in such scenarios.

To install `nvm`, visit the [nvm Github Page]. Below the code section, find the README for installation instructions. Typically, the README provides a special `curl` command to download and install `nvm` from the terminal. For example:

```shell
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash
```

Executing this command will display a series of messages, and the last three lines are crucial shell commands to initialize `nvm`.
```shell
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100 13527  100 13527    0     0  49731      0 --:--:-- --:--:-- --:--:-- 49915
=> Downloading nvm from git to '/home/your-user/.nvm'
=> Cloning into '/home/your-user/.nvm'...
remote: Enumerating objects: 333, done.
remote: Counting objects: 100% (333/333), done.
remote: Compressing objects: 100% (283/283), done.
remote: Total 333 (delta 38), reused 150 (delta 25), pack-reused 0
Receiving objects: 100% (333/333), 177.20 KiB | 1.46 MiB/s, done.
Resolving deltas: 100% (38/38), done.
=> Compressing and cleaning up git repository

=> Appending nvm source string to /home/your-user/.bashrc
=> Appending bash_completion source string to /home/your-user/.bashrc
=> Close and reopen your terminal to start using nvm or run the following to use it now:

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
```
To avoid running these commands every time you open a terminal, add them to your _shell startup file_.

The general rule is:
- If your shell is `zsh`, use `~/.zshrc`.
- If your shell is `bash`, use `~/.bashrc`.

To verify, open your startup file in Visual Studio Code using:

```shell
code ~/.zshrc
```

If the `nvm` startup lines are missing, add them manually. Run your startup file by either using the `source` command or by reopening your terminal window.

Once completed, run `nvm` at the command prompt; you should see help messages from `nvm`. If not, double-check your shell startup files.

## Installing Node.JS

Now that `nvm` is installed, use it to install Node.JS version 20:

```shell
nvm install 20
```
```shell
Downloading and installing node v20.10.0...
Downloading https://nodejs.org/dist/v20.10.0/node-v20.10.0.tar.gz...
######################################################################### 100.0%
Computing checksum with shasum -a 256
Checksums matched!
Now using node v20.10.0 (npm 10.2.3)
Creating default alias: default -> 20 (-> v20.10.0)
```
After completion, verify the Node.JS version:

```shell
node --version
```

Also, confirm that the Node.JS installation comes from your `nvm` setup:

```shell
which node
```

If the path contains `.nvm`, you've done it correctly. Congratulations on successfully installing Node.JS!

## Mocha - One Last Step

For testing your JavaScript code, you will use a tool called Mocha. Install it using the `npm` command:

```shell
npm install -g mocha
```

The `-g` flag indicates a global installation, making Mocha available for all projects. Verify Mocha installation by typing:

```shell
mocha --version
```

If it prints out a version number, congratulations, you have successfully installed Node.JS and Mocha!

[nvm Github Page]: https://github.com/nvm-sh/nvm
