`npm` Reference
=====================

## Contents
* [Basic Commands](#basic-commands)
* [Package Managing](#package-managing)

# Basic Commands

## Installing

```
npm install <package>[@version-number]
npm i <package>
```
* installs package locally, in the current directory.
* local installations installed into a `node_modules/` directory.

```
npm install -g <package-name>
```
* installs package globally and adds command to PATH

## Removing

```
npm remove <package>
```
* removes package

## Info

```
npm view <package>
```
* displays info, including `.tgz` file

# Package Managing

## `package.json` file

* Used to help maintain, update, and patch installed packages

* Makes `npm install` install all dependencies automatically

### Creating `package.json`

Type `npm init` then follow prompts(enter for default values)