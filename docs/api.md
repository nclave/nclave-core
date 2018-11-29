# Nclave API Reference

This is a general reference for the Nclave API. 

# Jargon:

### Core

Nclave without any aditional plugins or application logic. This includes the 
channel manager and the corresponding channels. The Nclave core can be built as
a client or a server.

### Channel

An array of handlers that the buffer passes through. At the end of each channel
there is an outboundcap handler and an inboundcap handler. 

The outboundcap handler transmittes the buffer to the specified host.

The inboundcap handler assignes the data of the buffer to a variable for
later use in the application.

### Connection

A connection from two Internet connected devices. A connection is analgous to 
an open socket connection between two devices. 

### Handler

Functions that take in data, mutate it and pass it down to the next handler or
to the app.

### App

The rest of the code in your network application. 

### Buffer

A fast and highly preformant data structure used to handle large amounts of 
binary data.

### Plugins

Third party dynamically loaded handlers or channels. Nclave comes with a few 
standard plugins to help you get started. Though many can be found
online. An index of popular plugins can be found 
[here](https://nclave.io/plugins/).