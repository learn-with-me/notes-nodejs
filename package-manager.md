# Package Manager

### NPM

#### Installation

###### Option 1

```
Option 4 -- Installs or updated NVM (Node Version Manager)
$ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.7/install.sh | bash
$ nvm install 8              # install node 8
$ nvm alias default 8        # to make node 8 the default
```

##### Cheatsheet

```
Save config in .npmrc
$ npm config set save=true
$ npm config set save-exact=true

You may want to use prexxx and postxxx scripts in package.json
```

#### NPX

A tool intended to let you run CLI of an NPM package without having to install them globally. NPX looks up in existing node\_modules for the folder to find the executable first. You could do that same thing by referencing `.bin` folder in command-line, however this tool makes it simpler. It comes bundled with NPM starting version 5.2.0 and onwards.

```
$ npx eslint .
```

### Yarn

#### Installation

###### Option 1

```
Install Yarn as Node's package manager. Also installs Node.js if not installed already.

$ brew install yarn
```

### Interesting packages to check out

```
https://www.npmjs.com/package/memwatch-next
https://www.npmjs.com/package/heapdump
https://www.npmjs.com/package/autocannon

```



