# Server Benchmarks

The idea behind this project is to measure performance over different operations across a wide variety of web frameworks. Over time we want to improve the coverage to cover a broad amount of frameworks.

If you would like to fix something, or add a new framework. Please feel free to send a PR my way.

# Testing Hardware

TODO

# Framework Endpoints

`/index` - Render a static template (index.html)  
`/index_json` - Render a static JSON (index.json)  
`/fortunes` - Read all fortune message from the DB, and render a template (fortunes.html)  
`/fortunes_json` - Read all fortune messages from the DB, and render JSON (fortunes.json)  

# File Structure

```
config/
- install.sh
- setup.sh
- *.sql

frameworks/
- language-name/
- - install.sh
- - framework-name/
- - - install.sh
- - - run.sh
- - - <framework-files>.*

templates/
- *.html
```

## config/

Configuration files for installing and setting up non framework specific tasks.

###### install.sh

Installing everything not framework specific, like `wrk2`, `postgresql`, etc.

###### setup.sh

Setup Database, etc.

## frameworks/

This directory contains all the frameworks to be tested.

### language-name/

This directory contains all the frameworks which use the same language.

###### install.sh

Install all language specific dependencies.

#### framework-name/

This directory contains framework specific files to setup the framework and run the tests.

###### install.sh

Install all framework specific dependencies.

###### run.sh

Run tests for this framework.

## templates/

Contains the various templates used.

# Running the tests
TODO

# Contributing
TODO

