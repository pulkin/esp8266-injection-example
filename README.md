[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=2RZCNXCUCP4YG&source=url)

# ESP8266 packet injection/sniffer example

**Warning!** This example runs with a particular SDK build that is now integrated into this project.
Future versions of the esp_iot_sdk removed the ability to send wifi control frames with `wifi_send_pkt_freedom`.
I recommend checking https://github.com/kieransimkin/esp8266-freedom for the relevant object files if you want to use both newer SDK and `wifi_send_pkt_freedom` the way it was implemented in this SDK build.

This example project utilizes sniffer capabilities of
ESP8266 to perform deauth attack. The communication between the
victim and access point (AP) is traced by `wifi_set_promiscuous_rx_cb`
while packet injection is performed by `wifi_send_pkt_freedom`.
To use the example adjust the Makefile and change MAC
addresses in user/user_main.c.
