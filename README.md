# Gauge example in Groovy
[![Build Status](https://travis-ci.org/getgauge-examples/gauge-example-groovy.svg?branch=master)](https://travis-ci.org/getgauge-examples/gauge-example-groovy)

This is an example project for doing web automation testing with [Gauge](http://getgauge.io). This project tests some of the functionalities of the [active admin demo](https://github.com/getgauge/activeadmin-demo) app. This app is hosted as a Java WAR (with embedded Jetty).

## Running this example
The tests are run on Firefox by default. You can set environment to run on different browsers.

### Prerequisites

This example requires the following softwares to run.
  * Java
  * [Gauge](http://getgauge.io/download.html)
  * Gauge Java plugin
    * Gauge Java plugin can be installed using `gauge --install java`

You can optionally install [Gauge-IntelliJ plugin](http://getgauge.io/documentation/user/current/ide_support/intellij_idea.html).

### Setting up the System Under Test (SUT)

* Download [activeadmin-demo.war](https://bintray.com/artifact/download/gauge/activeadmin-demo/activeadmin-demo.war)
* Bring up the SUT by executing the below command
```
java -jar activeadmin-demo.war
```
* The SUT should now be available at [http://localhost:8080/](http://localhost:8080)

### Execute specs

```
mvn clean test
```
This runs Gauge specs with [maven](https://maven.apache.org/).

Note:
  * Gauge can also be used with other [build tools](http://getgauge.io/documentation/user/current/test_code/java/using_build_tools.html) like gradle and ant.
  * You can use Gauge even without a build script!

## Topics covered in the example

* [Specification](http://getgauge.io/documentation/user/current/specifications/README.html), [Scenario](http://getgauge.io/documentation/user/current/specifications/scenarios.html),  [Step](http://getgauge.io/documentation/user/current/specifications/steps.html), [Concepts](http://getgauge.io/documentation/user/current/specifications/concepts.html) and [Context Steps](http://getgauge.io/documentation/user/current/specifications/contexts.html)
* [Table parameters](http://getgauge.io/documentation/user/current/specifications/parameters.html#table-parameter)
* Using [External datasource (special param)](http://getgauge.io/documentation/user/current/specifications/parameters.html#special-parameters)
* Using [tags](http://getgauge.io/documentation/user/current/specifications/tags.html)
* Using Gauge with [Selenium Webdriver](http://docs.seleniumhq.org/projects/webdriver/)
* Running Gauge specs with [maven](https://maven.apache.org/)
