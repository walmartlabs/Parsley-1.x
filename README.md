***
# NOTICE:

## This repository has been archived and is not supported.

[![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)
***
NOTICE: SUPPORT FOR THIS PROJECT HAS ENDED 

This projected was owned and maintained by Walmart. This project has reached its end of life and Walmart no longer supports this project.

We will no longer be monitoring the issues for this project or reviewing pull requests. You are free to continue using this project under the license terms or forks of this project at your own risk. This project is no longer subject to Walmart's bug bounty program or other security monitoring.


## Actions you can take

We recommend you take the following action:

  * Review any configuration files used for build automation and make appropriate updates to remove or replace this project
  * Notify other members of your team and/or organization of this change
  * Notify your security team to help you evaluate alternative options

## Forking and transition of ownership

For [security reasons](https://www.theregister.co.uk/2018/11/26/npm_repo_bitcoin_stealer/), Walmart does not transfer the ownership of our primary repos on Github or other platforms to other individuals/organizations. Further, we do not transfer ownership of packages for public package management systems.

If you would like to fork this package and continue development, you should choose a new name for the project and create your own packages, build automation, etc.

Please review the licensing terms of this project, which continue to be in effect even after decommission.

### WARNING: This page documents Parsley 1.x versions, which is NOT the latest stable release (2.x versions are). Unless you are here on purpose, you probably want to be viewing the latest documentation. Go to [parsleyjs.org](http://parsleyjs.org) for latest.

#Parsley.js 1.x

Javascript form validation, without actually writing a single line of javascript!

#TODOs

See TODO.md

#Curent Stable Version

1.2.4

# Browser compatibility

  - IE 7/8 (used with jQuery 1.x)
  - IE 9+ (latest jQuery and Zepto)
  - FF 14+
  - Chrome

# Min requirements

jQuery 1.7+

#Install dependencies for documentation and tests

`bower install jquery`
`bower install bootstrap`

#Run tests

* In your browser: go to `tests/index.html`
* Headless tests: install mocha-phantomjs with npm: `npm install -g mocha-phantomjs` and then run `./bin/test-suite.sh`

#Make production minified versions

You'll need ruby, and Google Closure compiler: `gem install closure-compiler`. Then, just call:

* Linux/Mac: `./bin/build.sh version` where version is the build release. eg: `./bin/build.sh 1.1.2`
* Windows: `./bin/build.ps1 version` where version is the build release. eg: `./bin/build.ps1 1.1.2`

They'll be created and dumped in the dist/ directory

#Contribute!

##Validators

Add new validators in `parsley.extend.js` and minify it. No validators will be allowed directly into parsley.js
(but great validators could move from extra to parsley ;))

##Localization

If file does not exist, create it into `ì18n/` directory with same syntax as others.
Reference file is _messages.en.js

##Integrations

Create integration with other framework as a separate Github repo and send a pull request for including here.
Some integrations are

* [Django](https://github.com/agiliq/django-parsley)
* [Rails](https://github.com/mekishizufu/parsley-rails)
* [Wicket](https://github.com/code-troopers/wicket-jsr303-parsley)
* [WTForms](https://github.com/johannes-gehrs/wtforms-parsleyjs)
* [Cascade Framework](https://github.com/jslegers/cascadeframework/)

##Conditional Logic

If you want to show and hide form elements based on answers to certain fields, the library below extends parsely.js adding conditional logic.

* [Parsely-conditions](http://themonk.github.io/parsely-conditions/)

## Global

* fork repository
* add your changes to parsley.js
* add / update tests to test suite (tests/index.html / tests/tests.js)
* run tests (see above)
* create new minified versions with minify script (see above) (use next tag-dev as version. Ie: if 1.1.1, use 1.1.2-dev)
* make a Pull Request!

#Licence

See LICENCE.md
