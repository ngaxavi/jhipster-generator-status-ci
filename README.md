# generator-jhipster-gitlab-ci-build-status
[![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] [![Dependency Status][daviddm-image]][daviddm-url]
> JHipster module, display the GitLab build status of your JHipster application into it 

<div align="center">
  <a href="http://jhipster.github.io">
    <img src="https://github.com/ngaxavi/generator-jhipster-gitlab-ci-build-status/raw/master/images/logo-jhipster.png">
  </a>
  <a href="https://about.gitlab.com/gitlab-ci/">
      <img width=93px src="https://github.com/ngaxavi/generator-jhipster-gitlab-ci-build-status/raw/master/images/gitlabci.png">
    </a>
</div>


# Introduction

This is a [JHipster](http://jhipster.github.io/) module, that is meant to be used in a JHipster application.
This module will add a view to the last build status of your application footer, when it deploys on GitLab.
After having push the code you just need to reload the page on your application to see the actual build status.

# Prerequisites

As this is a [JHipster](http://jhipster.github.io/) module, we expect you to have JHipster and its related tools already installed:

- [Installing JHipster](https://jhipster.github.io/installation.html)

Moreover you need your private token from GitLab. you can find it
```bash
Profile Settings -> Account -> Private Token
```
and you need the ID of your project from GitLab
```
Setting of your Project -> Triggers

and you will find something like this

curl -X POST \
     -F token=TOKEN \
     -F ref=REF_NAME \
     https://gitlab.com/api/v3/projects/123456/trigger/builds (project ID: 123456)
     
```

# Installation

To install this module:

```bash
npm install -g generator-jhipster-gitlab-ci-build-status
```

To update this module:
```bash
npm update -g generator-jhipster-gitlab-ci-build-status
```

# Usage
To run the module on a JHipster generated application: 
```bash
yo jhipster-gitlab-ci-build-status
```

# License

Apache-2.0 © [Xavier Ngansop]

[npm-image]: https://badge.fury.io/js/generator-jhipster-gitlab-ci-build-status.svg
[npm-url]: https://npmjs.org/package/generator-jhipster-gitlab-ci-build-status
[travis-image]: https://travis-ci.org/ngaxavi/generator-jhipster-gitlab-ci-build-status.svg?branch=master
[travis-url]: https://travis-ci.org/ngaxavi/generator-jhipster-gitlab-ci-build-status
[daviddm-image]: https://david-dm.org/ngaxavi/generator-jhipster-gitlab-ci-build-status.svg?theme=shields.io
[daviddm-url]: https://david-dm.org/ngaxavi/generator-jhipster-gitlab-ci-build-status
