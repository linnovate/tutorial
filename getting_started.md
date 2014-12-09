So before we dive in the first thing we need to do is to install mean.io.
Mean.io is based on mongo,express,angular and node and below are the explanations of what needs to be installed as a prerequiste before we get to business...
## Prerequisites
* *MongoDB* - <a href="http://www.mongodb.org/downloads">Download</a> and Install mongodb - <a href="http://docs.mongodb.org/manual">Checkout their manual</a> if you're just starting.
* *Node.js* - <a href="http://nodejs.org/download/">Download</a> and Install Node.js, nodeschool has free <a href=" http://nodeschool.io/#workshoppers">node tutorials</a> to get you started.
* *Git* - Get git using a package manager or <a href="http://git-scm.com/downloads">download</a> it.
* A taskrunner
    * Grunt - Download and Install [Grunt](http://gruntjs.com).
     ```
$ npm install -g grunt-cli
```
    * Gulp - Download and install
    ```
$ npm install -g gulp
```


## Installation
To start with MEAN install the `mean-cli` package from NPM.
This will add the *mean* command which lets you interact (install, manage, update ...) your mean based  application.

### Install the MEAN CLI

```bash
  $ sudo npm install -g mean-cli
  $ mean init <myApp>
  $ cd <myApp> && npm install
```

### Invoke node with Grunt
We recommend using [Grunt](https://github.com/gruntjs/grunt-cli) to start the server:
```bash
  $ grunt
```
If grunt aborts because of JSHINT errors, these can be overridden with the `force` flag:
```bash
  $ grunt -f
```
Alternatively, when not using `grunt` (and for production environments) you can run:
```bash
  $ node server
```
Then, open a browser and go to:
```bash
  http://localhost:3000
```