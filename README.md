<h1 align="center">INSTL <br> Automated GitHub Project Installer</sup></h1>

<p align="center">

<a style="text-decoration: none" href="https://github.com/installer/instl/releases">
<img src="https://img.shields.io/badge/platform-windows%20%7C%20macos%20%7C%20linux-informational?style=for-the-badge" alt="Downloads">
</a>

<a style="text-decoration: none" href="https://instl.sh/stats">
<img src="https://img.shields.io/endpoint?url=https://instl.sh/stats/total/badge/shields.io&style=for-the-badge" alt="Handeld Installations">
</a>

</p>

<p align="center">Instl is a install script generator that can handle most GitHub projects with a single command!</p>

<p align="center">
<img width="900" src="https://raw.githubusercontent.com/installer/instl/main/demo.gif" alt="Instl Demo">
</p>

----

<p align="center">
<strong><a href="https://docs.instl.sh">Documentation</a></strong>
|
<strong><a href="https://docs.instl.sh/contributing/writing-code">Contributing</a></strong>
</p>

----

## Web Installer

> The web install command can be used by anyone and does not require anything to be installed.  
> Running the web install command will download and install the given GitHub project.

The web installer is a single command, which everyone can run to install a GitHub project.
This is the basic syntax, which will return an install script from our API server:

                         ┌ The GitHub username of the project
                         |        ┌ The GitHub repository name of the project
                         |        |       ┌ The platform, see "Valid Platforms"
                         |        |       |
	https://instl.sh/username/reponame/platform

### Valid Platforms

| Valid Platforms | Parameter |
|-----------------|-----------|
|     Windows     |  windows  |
|      macOS      |  macos    |
|      Linux      |  linux    |

### Running the web installer command

> Different operating systems need different commands to download and run the web installer script.
> You can include those commands in your GitHub project, to provide a user-friendly installer for your CLI without any setup!

#### Windows

This command will download and execute the web installer script for windows.
You have to execute it in a powershell terminal.

```powershell
iwr instl.sh/username/reponame/windows | iex
```

#### macOS

This command will download and execute the web installer script for macOS.

```bash
curl -sSL instl.sh/username/reponame/macos | bash
```

#### Linux

This command will download and execute the web installer script for linux.

```bash
curl -sSL instl.sh/username/reponame/linux | bash
```
