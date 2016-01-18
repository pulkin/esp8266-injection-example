# ESP8266 packet injection/sniffer example

**Warning!** This example runs with a particular SDK build
which was available around September 2015. You can download it [here](https://www.dropbox.com/s/lkjwiyk81ky7wfu/esp_iot_sdk_v1.3.0_15_08_08.zip?dl=0).

This example project utilizes sniffer capabilities of
ESP8266 to perform deauth attack. Minimum SDK
requirement is 1.4.0. The communication between the
victim and access point (AP) is traced by `wifi_set_promiscuous_rx_cb`
while packet injection is performed by `wifi_send_pkt_freedom`.
To use the example adjust the Makefile and change MAC
addresses in user/user_main.c.
