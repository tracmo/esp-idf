set(COMPONENT_ADD_INCLUDEDIRS espmqtt/include)
set(COMPONENT_PRIV_INCLUDEDIRS "espmqtt/lib/include")
set(COMPONENT_SRCS "espmqtt/mqtt_client.c"
                   "espmqtt/lib/mqtt_msg.c"
                   "espmqtt/lib/mqtt_outbox.c"
                   "espmqtt/lib/platform_esp32_idf.c")

set(COMPONENT_REQUIRES lwip nghttp mbedtls tcp_transport)

register_component()
