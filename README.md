# React-native pods caching

## Introduction

Amount  of code in pods can be huge. Pods don’t change often. On CI, all pods are compiled over and over again, which is very time intensive. What if we compile Pods once and use the result over and over again? This repo contains a demo how to accomplish this.


## Setup

- clone this repo
- run `yarn install`
- `cd ios`
- run `pod install`
- run `gem install` (?)
- run `bundle exec fastlane ios build` for first time
- check build time, and notice existens of folder `cached_derived_data`
- run `bundle exec fastlane ios build` again
- check build time
