# Suricata IntelliSense Extension

The Suricata IntelliSense Extension is Visual Studio Code extension that uses the Suricata Language
Server to provide advanced syntax checking as well as auto-completion when editing Suricata signatures.

![VSCode Screenshot](https://raw.githubusercontent.com/StamusNetworks/suricata-ls-vscode/main/images/vscode-sample.png)

## Installation

The Suricata IntelliSense Extension can be installed from the Visual Studio Code Marketplace or from
the [GitHub project](https://github.com/StamusNetworks/suricata-ls-vscode)

The Suricata Language Server needs to be installed separately. See [Suricata Language Server page](https://github.com/StamusNetworks/suricata-language-server)
for specific instructions about its installation.

## Setup

For the settings on Microsoft Windows, you will need to escape the backslash in the paths you need to enter. With a standard Suricata MSI installation
and a standard installation of the server with ``pip`` the settings look like:

* Server Path: ``C:\\Users\\User\\AppData\\Local\\Programs\\Python\\Python310\\Scripts\\suricata-language-server.exe``
* Suricata Path: ``C:\\Program Files\\Suricata\\suricata.exe``

If you have Docker installed on your system, you can skip the installation of Suricata by checking
the `Container Mode` option. Suricata commands will then be run inside a container.

## Features

It provides auto-completion of Suricata keywords with access to the documentation:

![VSCode Completion](https://raw.githubusercontent.com/StamusNetworks/suricata-ls-vscode/main/images/vscode-completion.png)

The list of keywords is coming from Suricata so it will adapt automatically to the version you are using.

Advanced syntax check is done by Suricata on the signature files when they are saved. It also includes useful
hints such as the fast pattern that is picked by Suricata:

![VSCode Hint](https://raw.githubusercontent.com/StamusNetworks/suricata-ls-vscode/main/images/vscode-hint.png)

Syntax highlighting is not provided by this extension.
