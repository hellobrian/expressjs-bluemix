# Getting Started with Express.js on IBM Bluemix
This is a tutorial and boilerplate for creating websites and web apps with Express.js on IBM Bluemix

## Table of Contents

- [Pre-requisites](#pre-requisites)
  - [Install Node.js](#install-nodejs)
  - [Install CF-CLI](#install-cf-cli)
- [Setting up your project](#setting-up-your-project)
  1. [Create Package.json](#1-create-packagejson)
  2. [Install Express.js](#2-install-expressjs)
  3. [Add node_modules to .gitignore](#3-add-node_modules-to-gitignore)
- [Make a website with HTML]
  - [Manifest.yml]
- [Make a website with Dustjs Templates]
- [Using Routes]
- [Set up Gulp.js]


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

### 1. Create Package.json

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

**git commit**: Set up project, create package.json with npm init

[see commit](https://github.com/thisisbrianhan/expressjs-bluemix/commit/ec8155061833717f0278ee3e7e14f18fd4ed76b1)

### 2. Install Express.js

Install express: 

```
$ npm install express --save
```

`npm install` will install **express** and its dependencies inside a folder called `node_modules` in your app directory. 

The `--save` flag writes express into the dependencies section of your `package.json`.

**git commit**: Install express.js

[see commit](https://github.com/thisisbrianhan/expressjs-bluemix/commit/57079c1a01b4e9a529d7bcda95cf63f6de914fe1)

### 3. Add node_modules to .gitignore

When we deploy to Bluemix and when we check in our code to GitHub, we want to ignore the `node_module` folder because it's big. 

Specifically for deploying, Bluemix will use the dependencies listed in package.json to install express and other dependencies when it gets deployed to production. 

**git commit**: Add node_modules to .gitignore

[see commit](https://github.com/thisisbrianhan/expressjs-bluemix/commit/57079c1a01b4e9a529d7bcda95cf63f6de914fe1)

