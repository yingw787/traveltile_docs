---
date: 2016-03-09T00:11:02+01:00
title: Getting started
weight: 10
---

## Download

Clone the project from ```git```:

```sh
   git clone https://github.com/yingw787/traveltile_opensrc.git
```

## Setup

### Installation

Install NPM dependencies within the directory. Make sure you have up to date Node and NPM versions.

```sh
   cd traveltile_opensrc
   npm install
```

### Third-party APIs

This project relies on the Google Maps API, the FileStack API, and a running PostgreSQL instance. You can get a Google Maps API key from [the Google API Console](https://console.developers.google.com/), and you can get a FileStack API key from [their website](https://www.filestack.com/). If you use OS X, you can download and use [PostgresApp](http://postgresapp.com/), and if not (or if you prefer a global PostgreSQL instance), you can use [ElephantSQL](https://www.elephantsql.com/).

Fill in the API keys as follows:

- The PostgreSQL URL inside ```projectroot/config/applicationConfig.js```

- The Google Maps API key inside ```projectroot/public/js/config/apiKeys.js```

- The FileStack API key inside ```projectroot/public/js/models/EditorTilesModel.js```

### Remove demonstration mode

Currently, sections of ```projectroot/public/js/models/EditorTilesModel``` and ```projectroot/public/js/models/BrowserTilesModel.js``` are commented out as part of demonstration mode. In order to enable saving from the editor and deletion and editing from the browser, said code blocks must be uncommented.

## Usage

In your Terminal, type

```sh
   npm run start
```

In order to start Webpack and run the project. Open up your browser, go to ```localhost:8080``` in order to see the application in action!

## Questions/Comments/Concerns

Please submit any questions, comments, or concerns about this setup procedure as an [issue](https://github.com/yingw787/traveltile_opensrc/issues) on the repository.
