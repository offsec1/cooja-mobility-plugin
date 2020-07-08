# Cooja Mobility Plugin
This repository contains the mobility plugin for Cooja. 
It helps to simulate VANETs using Cooja.


## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
---

## Installation
### Clone
- Clone this repo to your local machine into the apps folder of the Cooja installation path `~/contiki-ng/tools/cooja/apps` using `https://github.com/offsec1/mobility`

### Setup
Before starting Cooja you have to build the .jar file for the plugin. Run following command inside the mobility directory

```shell
$ ant jar
```
---

### Cooja settings
Now start Cooja and goto Settings -> External Tools Path...

- Edit DEFAULT_PROJECTDIRS
- At the end add following string `;[CONTIKI_DIR]/tools/cooja/apps/mobility`
- Restart Cooja and under Tools you should see a new entry called Mobility

## Usage
Changing the position.dat

    * Quit Cooja
    * Replace position.dat
    * Clean and rebuild the plugin
        cd contiki-folder/tools/cooja/apps/mobility
        ant clean
        ant jar
    * Start Cooja and run your simulation...
---
