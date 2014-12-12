JTAF-XCore [![Build Status](https://secure.travis-ci.org/FINRAOS/JTAF-XCore.png?branch=master)](http://travis-ci.org/FINRAOS/JTAF-XCore)
==================
[XCore](http://finraos.github.io/JTAF-XCore/) is a test framework allowing for someone to define tests in XML 'test scripts' after a Java developer develops the code behind executing the steps.

Click here to [get started](http://finraos.github.io/JTAF-XCore/howitworks.html)!

Releases
========
>[Release 1.0](https://github.com/FINRAOS/JTAF-XCore/releases/tag/jtaf-xcore-1.0) is available on Maven central repository! - 12/5/2014

>Release 1.1 - Coming soon!

Contributing
=============
We encourage contribution from the open source community to help make XCore better. Please refer to the [development](http://finraos.github.io/JTAF-XCore/contribute.html) page for more information on how to contribute to this project including sign off and the [DCO](https://github.com/FINRAOS/JTAF-XCore/blob/master/DCO) agreement.

If you have any questions or discussion topics, please post them on [Google Groups](https://groups.google.com/forum/#!forum/jtaf-xcore).

Building
=========
XCore uses Maven for build. Please install Maven by downloading it [here](http://maven.apache.org/download.cgi).
```sh
# Clone XCore git repo
git clone git://github.com/FINRAOS/JTAF-XCore.git
cd JTAF-XCore/seedProject

# Run verify to execute some tests
mvn verify
```

Running Tests
==============
XCore uses JUnit to run its tests. To start out, jtaf.properties will need to get [defined](http://finraos.github.io/JTAF-XCore/properties.html) in order to choose what tests to run and how to run them. Running XMLTestDriver with JUnit from your IDE or command line will execute the tests as determined by the [strategy](http://finraos.github.io/JTAF-XCore/strategy.html) in the jtaf.properties run configuration.

Once you're ready, XCore allows easy setup to run test suites on the CI ([like Jenkins](http://www.jenkins-ci.org/)) by setting run configuration properties as System variables. Setting the run configuration properties as System variables will override what's defined in jtaf.properties.

```sh
# Run verify to run the tests on the CI
mvn verify
```

Requirements
==============
XCore requires Java SE version 7 or above available [here](http://www.oracle.com/technetwork/java/javase/downloads/index.html).

License Type
=============
JTAF projects including XCore is licensed under [Apache License Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)