# Nclave - Modern and useful network framework

Nclave is a network framework that helps one develop safe and secure 
network applications quicker with less work. Nclave is cross-platform and 
cross-language by default. While the core is written in Rust, Nclave was 
designed for cross compatibility. 

Nclave is non blocking by default and completley asynchronous. This allows for
management of many connections on less resources than conventional network
libraries. Nclave is designed for applications that have many concurrenct 
connections, require low latency with minimal overhead. 

More information can be found in the docs directory and 
[here](https://nclave.io/docs/en/v0.0.1/).

# Motivation

The motivation for Nclave is the state of network programming as of 2018.
Besides some outliers, network programming is dominated by the Berkley Sockets
API. Many applications that communicate over the Internet communicate over HTTP
which leads to byzantine protocols such as websockets. 

Nclave intends to be a framework that is made for humans who want to write fast,
secure, and clean network applications without sacrificing time and resources.

# Plugins

Nclave has native support for plugins through dynamic loading. Many common and 
useful plugins have been created for reuse in any project. More infomation can
be found [here](https://nclave.io/plugins/).

# Installing

To install Nclave into your project, install the 
[Nclave Manager](https://github.com/nclave/nclave-manager) and initialize 
the project. 

```bash 
$ ncl init project_name
```

From there the nclave directory will be created and will have the object 
files needed for functionality of the application. Also the config file
nclave.conf will be created for configuring Nclave.

After that, it is as simple as including or importing the respective header into 
your code and calling the Nclave API.

A more indepth tutorial on getting started can be found 
[here](https://nclave.io/docs/en/v0.0.1/getting-started/).

# Contributing

To contribute to Nclave see CONTRIBUTING.

# License

Nclave is licensed in GPLv2. For more information see LICENSE.
