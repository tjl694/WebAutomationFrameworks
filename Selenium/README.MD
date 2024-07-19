# Selenium WebDriver in JavaScript framework

This automation uses a Selenium WebDriver framework in JavaScript using [selenium-cucumber-js](https://github.com/john-doherty/selenium-cucumber-js).

### Installation

This requires [Node.js](https://nodejs.org/) to run.
1. Clone the repo
2. ```cd``` into the folder you just cloned into
3. Run ```npm install```

### Running the framework
```sh
npm run test
```
It defaults to running in Chrome, but this can be switched to Firefox in the ```browser``` key value of ```./selenium-cucumber-js.json``` file.
### Reporting
Once ```npm run test``` has finished, a HTML report, ```cucumber-report.html```, will be available in the ```reports``` folder.

### Understanding the framework
There are 3 main folders
- ```features``` - home of the gherkin/cucmber steps
- ```step-definitions``` - home of the gherkin step definitions and functions
- ```page-objects``` - home of the defined elements for pages and any other functions

Also, there are a couple of config files
- ```./selenium-cucumber-js.json``` - this contains config values for the framework
- ```./config.json``` - this contains config values for the automation scripts to use, i.e. URLs

### Todo
- Implement automatic retry if Scenario fails (to a limited number of retries)
- Implement argument parsing within the package.json script for running specific Tags

License
----
MIT
