# How the Sesam Community works

This Github account is used to maintain and build reusable open source extensions for Sesam.

The Docker images are built and deployed to
 - https://hub.docker.com/r/sesamcommunity/ , when it is a sesam-community repo
or
 - https://hub.docker.com/r/[contributer]/ , when it is a contributers repo

## Requirements for repositories

- The extension require a LICENSE file that makes this process legal
- The extension should be usable from within Sesam
- The extension should be reusable
- The README file should contain an example
- The CI&CD should be implemented as described below

## How to contribute?

You can contribute either
 - by forking an existing repo or
 - if it is a new repo, by contacting a community member to get your repo forked into sesam-community

## How to setup?

Steps to build your own setup:
* Sign up at Dockerhub if you don't have an account
* Prepare your repo & branch
* Add git action 'Sesam Community CI&CD Workflow'
  * Add your DOCKER_USERNAME and DOCKER_PASSWORD as secrets to your git repository(Settings>Secrets)
  * The CI&CD workflow will build docker image for all push-to-master, releases and PRs. The image will be pushed to dockerhub with tag 'development' if it is a push-to-master and with the release tag when it is a release.
* Share your improvements using Pull Requests 

## FAQ

##### Q: I want you to build and deploy my extension as well!
A: Just send an email to baard.johansen@sesam.io with a link to the repository and we'll sort it out!
