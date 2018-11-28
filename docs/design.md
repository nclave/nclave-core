# Nclave API Reference

This is a general reference for the Nclave API. 

# Introduction

To first understand the Nclave API, one has to understand the architecture of 
the framework. 

# Jargon

Some technical jargon with Nclave:

### Core

Nclave without any additional plugins or 

### Channel

A linked list of handlers that the data passes through.

### Connection

A connection from two Internet connected devices

### Handler

Functions that take in data, mutate it and pass it down to the next handler or
to the app.

### App

The rest of the code in your network application 

### Data 

The information sent over the Internet.

### Plugins

Third party dynamically loaded handlers.


# The Nclave channel

The logic of your app will be defined outside of Nclave. Nclave defines the 
channels for the network stack of your application. A channel is a list of 
handlers that can mutate the data that is passed through them. 