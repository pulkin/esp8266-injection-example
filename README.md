# ESP8266 packet injection/sniffer example

**Warning!** This example runs with a particular SDK build that is now integrated into this project.
Future versions of the esp_iot_sdk removed the ability to send wifi control frames with `wifi_send_pkt_freedom`.

This example project utilizes sniffer capabilities of
ESP8266 to perform deauth attack. The communication between the
victim and access point (AP) is traced by `wifi_set_promiscuous_rx_cb`
while packet injection is performed by `wifi_send_pkt_freedom`.
To use the example adjust the Makefile and change MAC
addresses in user/user_main.c.
