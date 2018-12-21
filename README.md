# Using JMeter to load test

## Linux VM on Azure
<https://docs.microsoft.com/en-us/azure/virtual-machines/linux/quick-create-portal> - setup guide

## Linux VM setup and sample run JMeter

1. JDK

```
$ sudo apt-get install openjdk-8-jre
```
<https://openjdk.java.net/install/index.html>

2. JMeter

```
$ wget -c http://mirror.cc.columbia.edu/pub/software/apache//jmeter/binaries/apache-jmeter-5.0.tgz
$ tar -xvf apache-jmeter-5.0.tgz
```
<https://jmeter.apache.org/download_jmeter.cgi> - downloads page

3. JMeter Test

```
$ apache-jmeter-5.0/bin/jmeter -n -t apache-jmeter-5.0/extras/Test.jmx
```

## JMeter Test Plan creation

<https://jmeter.apache.org/usermanual/build-web-test-plan.html> - test plan

## Misc Links

<https://jmeter.apache.org/usermanual/build-web-test-plan.html> - test plan
<https://www.digitalocean.com/community/tutorials/how-to-use-apache-jmeter-to-perform-load-testing-on-a-web-server> - load testing
<https://jmeter.apache.org/usermanual/get-started.html> - getting started with jmeter
  - runs with heap of 1GB, may not be enough depending on test plan and number of threads
<https://github.com/department-of-veterans-affairs/ascent-sample/wiki/QA-:-Performance-Test-Plan-using-JMeter> - jmeter

### Example of load testing

<https://blog.kubernauts.io/load-testing-as-a-service-with-jmeter-on-kubernetes-fc5288bb0c8b> - jmeter load testing with kubernetes, distributed
  - simulate hundreds of thousands of simultaneous users
  - distributed load test
  - https://github.com/kubernauts/jmeter-kubernetes - scripts, etc
