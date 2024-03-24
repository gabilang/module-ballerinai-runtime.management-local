Ballerina Runtime-Management Internal Module
=====================================

  [![Build](https://github.com/ballerina-platform/module-ballerinai-transaction/actions/workflows/build-timestamped-master.yml/badge.svg)](https://github.com/ballerina-platform/module-ballerinai-transaction/actions/workflows/build-timestamped-master.yml)
  [![GitHub Last Commit](https://img.shields.io/github/last-commit/ballerina-platform/module-ballerinai-transaction.svg)](https://github.com/ballerina-platform/module-ballerinai-transaction/commits/master)
  [![Github issues](https://img.shields.io/github/issues/ballerina-platform/module-ballerinai-transaction.svg?label=Open%20Issues)](https://github.com/ballerina-platform/module-ballerinai-transaction/issues)
  [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
  [![codecov](https://codecov.io/gh/ballerina-platform/module-ballerinai-transaction/branch/master/graph/badge.svg)](https://codecov.io/gh/ballerina-platform/module-ballerinai-transaction)
  [![GraalVM Check](https://github.com/ballerina-platform/module-ballerinai-transaction/actions/workflows/build-with-bal-test-graalvm.yml/badge.svg)](https://github.com/ballerina-platform/module-ballerinai-transaction/actions/workflows/build-with-bal-test-graalvm.yml)

The Ballerina runtime.management internal module defines a service to expose runtime artifacts like deployed services, 
configurable variables, and resources to control runtime artifacts. Once the user defines the configurations 
inside Ballerina.toml, the management module will be imported to the user's project.


During initialization, the ballerina node will be registered in the integration control plane using configurations 
in Ballerina.toml. Then the integration control plan will connect with a given node via a service the module exposes 
to discover and control artifacts.


## Building from the Source

### Setting Up the Prerequisites

1. Download and install Java SE Development Kit (JDK) version 17 (from one of the following locations).
   * [Oracle](https://www.oracle.com/java/technologies/downloads/)
   * [OpenJDK](http://openjdk.java.net/install/index.html)

2. Export Github Personal access token with read package permissions as follows,
        
        export packageUser=<Username>
        export packagePAT=<Personal access token>

### Building the Source

Execute the commands below to build from the source.

1. To build the library:
        
        ./gradlew clean build

2. To run the integration tests:

        ./gradlew clean test

3. To build the module without tests:

        ./gradlew clean build -x test

4. To debug the tests:

        ./gradlew clean build -Pdebug=<port>

## Contributing to Ballerina

As an open source project, Ballerina welcomes contributions from the community. 

For more information, go to the [contribution guidelines](https://github.com/ballerina-platform/ballerina-lang/blob/master/CONTRIBUTING.md).

## Code of Conduct

All contributors are encouraged to read the [Ballerina Code of Conduct](https://ballerina.io/code-of-conduct).

## Useful Links

* Discuss about code changes of the Ballerina project in [ballerina-dev@googlegroups.com](mailto:ballerina-dev@googlegroups.com).
* Chat live with us via our [Discord server](https://discord.gg/ballerinalang).
* Post all technical questions on Stack Overflow with the [#ballerina](https://stackoverflow.com/questions/tagged/ballerina) tag.
