---
title: npm
---

# NPM

- package management tools
- managing dependencies
- running tasks
- publishing packages

## npm init

```bash
  npm init -y
```

creates a new `package.json` file

## package.json

```json
  {
    "name": "my-project",
    "version": "1.0.0",
    "dependencies": {
      "node-fetch": "^3.1.4"
    },
    "devDependencies": {
      "chai": "",
    }
  }
```

## npm install

```bash
  npm i -S package1 package2
```
will download and install the given packages
and save them as dependencies in your `package.json`
```bash
  npm i -D packageNames
```
will instead add the dependencies as `devDependencies`

## npm ls

```bash
  npm ls
```

will list all installed packages.
Warns you for packages not present in your `package.json`

## semantic versions

`major.minor.patch`

- A major version change reflects a change in the public API of the module
- A minor version change reflects adding new functionality
- A patch version change reflects improvements, bug and security fixes
