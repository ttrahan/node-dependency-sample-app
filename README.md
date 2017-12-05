![AyeAye](https://github.com/shippableSamples/node-build-push-docker-hub/blob/master/public/resources/images/captain.png)


## Dependencies

What you need to run this app:

* [Node.Js](https://nodejs.org)

## Instructions

### Setup

* Clone this repo:   
```
$ git clone https://github.com/ttrahan/node-dependency-sample-app.git
```

* Change into the app directory:
```
$ cd node-dependency-sample-app
```

* Install the dependencies (from the command line):  
```
$ npm install
```

Note, this will install a module dependency from:
https://github.com/ttrahan/node-dependency-sample-module.git
  * You can clone this dependency into your account, just update the package.json 
file in the root of this repo with the new location.

When finished, you should see the following tree structure:
```
.
├── README.md
├── example.js
├── node_modules
│   └── dateTools
│       ├── README.md
│       ├── index.js
│       └── package.json
├── package.json
└── shippable.yml
```

### Run the example app from the command line

```
$ node example.js
```

## Using with Shippable
To run this example in Shippable:
1. Clone both repos and [enable them for CI](http://docs.shippable.com/ci/enable-project/) in Shippable
2. Add the [Deployment Key](http://docs.shippable.com/platform/management/subscription/settings/#viewing-subscription-settings) from Shippable to the repo holding in your SCM the module code 
3. Add a [syncRepo](http://docs.shippable.com/platform/tutorial/workflow/crud-syncrepo/#adding-a-syncrepo) for the workflow configuration in the app repo
4. Commit changes to either repo or [manually run](http://docs.shippable.com/platform/visibility/single-pane-of-glass-spog/#runpause-job) a build from the SPOG view




