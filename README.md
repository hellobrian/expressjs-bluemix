# Getting Started with Express.js on IBM Bluemix
This is a tutorial and boilerplate for creating websites and web apps with Express.js on IBM Bluemix

## Pre-requisites 
You need node.js and CF-CLI (cloudfoundry commandline tool). 
You should also be using Git and GitHub - p

### Install Node.js
For windows users, install node.js here. 
**Mac users**: my preferred way of getting Node.js is via Homebrew, a package manager for mac. 
Follow the instructions on the site and you can install node.js via terminal: 
```bash
$ brew install node
```

### Install CF-CLI
For windows users, install CF-CLI here
**Mac users**: we can also use Homebrew to instal CF-CLI
```bash
$ brew tap pivotal/tap
$ brew install cloudfoundry-cli
```

## Setting up your project 

### 1. npm init

In your terminal, create a directory for your app and `cd` into it. 
For now, we're going to call it expressjs-bluemix, but pick whatever name you want. 
```bash
$ mkdir expressjs-bluemix
$ cd expressjs-bluemix
```
Then we're going to create a package.json file with the `npm init` command: 
```bash
$ npm init
```
Keep pressing enter to accept the defaults for the package.json. 

You'll have a package.json file that looks like this: 
```json
{
  "name": "expressjs-bluemix",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "",
  "license": "ISC"
}
```

I've slightly edited my package.json with some info about my app. 
Open up your project in your text editor, and feel free to make changes to the package.json: 

```json
{
  "name": "expressjs-boilerplate",
  "version": "1.0.0",
  "description": "this is an expressjs boilerplate to use for getting started with website or web app prototypes to deploy on IBM Bluemix",
  "main": "app.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [
    "expressjs",
    "Bluemix",
    "IBM"
  ],
  "author": "Brian Han",
  "license": "MIT"
}
```

Now's a good time for a commit: 

```git
Set up project, create package.json with npm init
```
[see commit](https://github.com/thisisbrianhan/expressjs-bluemix/commit/ec8155061833717f0278ee3e7e14f18fd4ed76b1)
