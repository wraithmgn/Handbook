## Wi-Fi

The WifiInterface provides a simple C++ API for connecting to the internet over a Wi-Fi device.

There are multiple [Wi-Fi components](https://os.mbed.com/components/cat/wifi/) that implement the WiFiInterface class. The example below uses the [ESP8266Interface](https://github.com/armmbed/esp8266-driver).

### Wi-Fi class reference

[![View code](https://www.mbed.com/embed/?type=library)](http://os-doc-builder.test.mbed.com/docs/development/mbed-os-api-doxy/class_wi_fi_interface.html)

### Usage

To bring up the network interface:

1. Instantiate an implementation of the WiFiInterface class (for example, the ESP8266Interface).
1. Call the `connect` function with an SSID and password for the Wi-Fi network.
1. Once connected, the WiFiInterface can be used as a target for opening [network sockets](/docs/development/reference/network-socket.html).

### Wi-Fi example

Here is an example of an HTTP client program. The program brings up an ESP8266 as the underlying network interface, and uses it to perform an HTTP transaction over a TCPSocket:

[![View code](https://www.mbed.com/embed/?url=https://os.mbed.com/teams/mbed_example/code/TCPSocketWiFi_Example/)](https://os.mbed.com/teams/mbed_example/code/TCPSocketWiFi_Example/file/6a4e57edc2b2/main.cpp)

### Related content

- [Wi-Fi components](https://os.mbed.com/components/cat/wifi/).
- [Network socket](/docs/development/reference/network-socket.html) API overview.
