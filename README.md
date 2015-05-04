# Backbase Launchpad-CLI tools

Backbase Launchpad tools for widgets / modules 

# Information
| name                  | version       | node      |
| ----------------------|:-------------:| ----------:|
| backbase              | 0.0.1         | >= 0.10    |


## Requirements
- git
- nodejs
- bower
- curl

## Install

```
npm i bb-lp-cli -g 
```

## Usage

Using **bblp** as binary.


### Generate widget/module:

arguments:
    - url 'repo url'
options:
- **NONE**

```bash
bblp generate <url>
```

### Install bower dependencies:
arguments:

- **&lt;package-name&gt;**

options:

- **NONE**

```bash
bblp install
```


### Start local server: http://localhost:3000

arguments:

- **NONE**

options:

- **l --link** auto link dependencies (if they are already linked)
    

```bash
bblp start
```

### Test: 
arguments:

- **NONE**

options:
- **w --watch** watch test files and source files

```bash
bblp test
```


### Build: 

arguments:
    
- **NONE**

options:

- **- s --skipTests** skips unit tests

```bash
bblp build
```


### Register: Register bower package to registry endpoint

arguments:

- **registry** - registry url default is http://launchpad.backbase.com:5678

options:
- **NONE**

```bash
bblp register
```

### Unregister: Unregister bower package to registry endpoint
arguments:

- **registry** - registry url default is http://launchpad.backbase.com:5678

options:

- **NONE**

```bash
bblp unregister
```

### Configuration under the bower.json file

This is the default config structure if is not specified otherwise in **bower.json** file


```javascript
"config": {
    "paths" : {
        "scripts": "./scripts",
        "docs": "./docs",
        "target": "./dist",
        "templates": "./templates",
        "styles": "./styles",
        "test": "./test",
        "index": "./index-dev.html"
    },

    "proxies": {
      "/api":  "http://localhost:3030/"
    }
    ....    
}
```


## TODO:


Commands
- bblp docs (generate documentation)
- bblp bump (bump the verion)
- bblp package (generate a zip package from dist folder)

Output
- better output
- use debug flag

Test
- add tests


## Contributing
 tba
