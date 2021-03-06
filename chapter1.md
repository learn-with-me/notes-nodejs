# Installation

### Mac OSX

##### Installation Path

```
Node.js - /usr/local/bin/node
NPM     - /usr/local/bin/npm
```

##### Option 1

```
Option 1
$ curl "https://nodejs.org/dist/latest/node-${VERSION:-$(wget -qO- https://nodejs.org/dist/latest/ | sed -nE 's|.*>node-(.*)\.pkg</a>.*|\1|p')}.pkg" > "$HOME/Downloads/node-latest.pkg" && sudo installer -store -pkg "$HOME/Downloads/node-latest.pkg" -target "/"
```

##### Option 2

```
$ brew install node      // Install
$ brew install node@8    // Install specific version
$ brew uninstall node    // Uninstall

General steps involved using brew
$ brew search node // This can return you multiple versions of node with one selected as default
$ brew unlink node // If you have latest package installed, unlink it first
$ brew install node@7 // Install the desired version, if not already done
$ brew link node@7 // Then link the desired version
$ node --version // confirm the node version if everything went correctly
```

##### Option 3

```
Install Yarn as Node's package manager. Also install Node.js if not installed already.

$ brew install yarn
```

##### Option 4 - Installs or updates NVM \(Node Version Manager\)

```
$ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.7/install.sh | bash
$ nvm install 8              # install node 8
$ nvm alias default 8        # to make node 8 the default
```

#### Reference

```
Reference: http://sourabhbajaj.com/mac-setup/Node.js/

```



