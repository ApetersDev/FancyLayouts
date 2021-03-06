FancyLayouts Vaadin UI Component Add On

FancyLayouts are fancy layouts and components which add transitions to normal
vaadin counterparts.

Demo application: http://siika.fi:8080/FancyLayoutsDemo
Source code: https://github.com/alump/FancyLayouts
Vaadin Directory: http://vaadin.com/directory#addon/fancylayouts
License: Apache License 2.0

This project can be imported to Eclipse with m2e.

Simple Maven tutorials:


***** How to compile add on jar package for your project *****

> cd fancylayouts-addon
> mvn package

add on can be found at: addon/target/FancyLayouts-<version>.jar
zip package used at Vaadin directory can be found at:
addon/target/FancyLayouts-<version>.zip

***** How to install fancylayouts to your Maven repository *****

To install addon to your local repository, run:

> cd fancylayouts-addon
> mvn install


***** How to run test application *****

First compile and install addon (if not already installed)
> cd fancylayouts-addon
> mvn install

Then compile demo widgetset and start HTTP server
> cd ../fancylayouts-demo
> mvn vaadin:compile
> mvn jetty:run

Demo application is running at http://localhost:8080/fancylayouts



***** How to compile test application WAR *****

First compile and install addon (if not already installed)
> cd fancylayouts-addon
> mvn install

Then construct demo package (this should automatically compile widgetset)
> cd ../fancylayouts-demo
> mvn package

War package can be now found at demo/target/FancyLayoutsDemo.war
