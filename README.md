# ESP8266 packet injection/sniffer example

This example project utilizes sniffer capabilities of
ESP8266 to perform deauth attack. Minimum SDK
requirement is 1.4.0. The communication between the
victim and access point (AP) is traced by `wifi_set_promiscuous_rx_cb`
while packet injection is performed by `wifi_send_pkt_freedom`.
To use the example adjust the Makefile and change MAC
addresses in user/user_main.c.
