# Home Assistant Add-on: Zigbee2MQTT-2

# MQTT
#base_topic多加一个2 以此类推

#client_id多加一个2 以此类推

```shell
mqtt:
  base_topic: zigbee2mqtt2
  server: mqtt://localhost:1883
  user: mqtt
  password: mqtt
  client_id: zigbee2mqtt2
```

# 信道
```shell
advanced:
  channel: 11 #信道要分开 选15 20 25
  #UI设置z2m设置→高级→ZigBee channel
```
