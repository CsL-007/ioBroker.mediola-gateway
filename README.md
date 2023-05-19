![Logo](admin/mediola-gateway.png)

# ioBroker.mediola-gateway

[![NPM version](https://img.shields.io/npm/v/iobroker.mediola-gateway.svg)](https://www.npmjs.com/package/iobroker.mediola-gateway)
[![Downloads](https://img.shields.io/npm/dm/iobroker.mediola-gateway.svg)](https://www.npmjs.com/package/iobroker.mediola-gateway)
![Number of Installations](https://iobroker.live/badges/mediola-gateway-installed.svg)
![Current version in stable repository](https://iobroker.live/badges/mediola-gateway-stable.svg)

[![NPM](https://nodei.co/npm/iobroker.mediola-gateway.png?downloads=true)](https://nodei.co/npm/iobroker.mediola-gateway/)

**Tests:** ![Test and Release](https://github.com/oelison/ioBroker.mediola-gateway/workflows/Test%20and%20Release/badge.svg)

## mediola-gateway adapter for ioBroker

Configuration and usage of Mediola-Gateways

## usage with e.g. mediola gateway V4

When you have only one Mediola Gateway (https://www.mediola.com/), auto detection is the best way to get started. In the logs the detected IP-Address and MAC-Address is after detection visible. When you have more then one Mediola Gateways, it is better to give the adapter the MAC-Address. Then this specific Gateway will be found. It is also possible to use the IP-Address, when this is not changing and better known than the MAC-Address.
After the adapter has found the Mediola Gateway, the instance become green and the objects receivedIrData, sendIrData and sendRfData are usable. When you have sys vars in the Mediola Gateway, they will be listed also in the object list. After some time, mostly the receivedIrData is changing. This represents the received IR date in the room, where the Mediola Gateway is located.
Every change of the sys vars will also be shown there and could be used for automation.
The sendIrData is tested with several learned IR codes. Just putting the IR code into the object to send the data.

### DISCLAIMER

DISCLAIMER All product and company names or logos are Trademarks™ or Registered® Trademarks of their respective owners. Their use does not imply any Affiliation or endorsement by them or associated affiliates! This personal project is being pursued on a recreational basis and Has no business objectives. mediola is a trademark of mediola - connected living AG.

## Changelog

<!--
    Placeholder for the next version (at the beginning of the line):
    ### **WORK IN PROGRESS**
-->

### **WORK IN PROGRESS**

-   axios with log error on error
-   ack true for readonly objects
-   ack check on state change
-   invalid chars checked

### 0.1.3 (2023-05-18)

-   test and release script corrected

### 0.1.2 (2023-05-18)

-   npm deploy activated
-   Readme improved

### 0.1.1 (2023-05-11)

-   dependencies update

### 0.1.0 (2023-05-03)

-   initial release
-   send ir (only IR_ID 01 front IR)
-   reveive ir

## License

MIT License

Copyright (c) 2023 oelison <iobrokermediola@sciphy.de>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
