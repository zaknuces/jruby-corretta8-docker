# jruby-corretta8-docker
A simple repo that contains a dockerfile for jruby image based on amazon-corretta8

## Secure
The docker image in this repo is created by taking TwistLock Scans into account. Following are the security compliance status based on standard jruby docker (based on OpenJDK 8)

### Jruby Standard Docker image Scan status
```
  "vulnerabilityDistribution": {
    "critical": 0,
    "high": 16,
    "medium": 26,
    "low": 66,
    "total": 108
  }
```

### This Jruby Docker image Scan Status
```
  "vulnerabilityDistribution": {
    "critical": 0,
    "high": 0,
    "medium": 10,
    "low": 0,
    "total": 10
  }
```

## Build
This repo is linked to [Official Docker Image](https://hub.docker.com/r/owaiszahid/jruby-corretta8-docker). Any change to master branch will trigger a new build

## TODOs
1. There are 10 medium vulnerabilities that can be address by updating the base image of amazoncorretta. See details [here](https://github.com/amazonlinux/container-images/issues/30)
2. To keep the image slim, we also like to create JRE based image. See details [here](https://github.com/corretto/corretto-8-docker/issues/17)
