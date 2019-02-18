# Cheatsheet

#### Node

```
$ node                        # Opens up Node REPL in command line
> .save index.js              # Saves REPL session into a file
> .load index.js              # Loads content of a file into Node REPL
> c <tab> <tab>               # Lists all possible combination for the letter C or anything you type
$ node index.js               # Runs a js script (index.js in this case)

$ node -p "some string"       # Executes a string expression
$ node -p "os.cpus().length"
$ node -p "process.versions.v8"
$ node -p "process.argv" hello 42

$ node -h | less              # Help on node
$ node --v8-options | grep "in progress"
$ NODE_DEBUG="http,fs" node index.js
$ VAL1=10 node index.js       # Sets a variable key-value in process.env
    $ export VAL1=10          # works same as above, just two steps
    $ node index.js

```

#### NPM

```
$ npm list -g --depth=0        # List all global dependencies
$ npm config list              # Display Node and NPM configs
```

#### Methods

```
setTimeout, clearTimeout, setImmediate, clearImmediate, setInterval, clearInterval
setTimeout(0) = setImmediate
setTimeout - returns the timerId
clearTimeout(timerId) - cancels out the timeout
time in setTimeout is a minimum time, since operation can be blocked by a blocking lines of code (for loop)

console.log == process.stdout.write

process.on('exit', () => {})
```



