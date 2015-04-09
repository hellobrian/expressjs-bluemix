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

### npm init

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
Open up your project in your text editor. 
When you [see my first commit](https://github.com/thisisbrianhan/expressjs-bluemix/commit/ec8155061833717f0278ee3e7e14f18fd4ed76b1), y
you'll see that I've edited it slightly.
