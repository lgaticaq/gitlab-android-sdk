# gitlab-android-sdk

[![dockeri.co](http://dockeri.co/image/lgatica/gitlab-android-sdk)](https://hub.docker.com/r/lgatica/gitlab-android-sdk/)

[![Build Status](https://travis-ci.org/lgaticaq/gitlab-android-sdk.svg?branch=master)](https://travis-ci.org/lgaticaq/gitlab-android-sdk)

> Docker image for build android apps in gitlab ci

## Create a .gitlab-ci.yml
```yml
image: lgatica/gitlab-android-sdk

before_script:
  - chmod +x ./gradlew

build:
  script:
    - ./gradlew assembleDebug
  artifacts:
    paths:
    - app/build/outputs/
```
