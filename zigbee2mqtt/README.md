# Home Assistant Add-on: Zigbee2MQTT-2

MQTT:

base_topic多加一个2 以此类推

client_id多加一个2 以此类推

```shell
mqtt:
  base_topic: zigbee2mqtt2
  server: mqtt://localhost:1883
  #mqtt在Home Assistantaz 安装，localhost是Home Assistantaz的ip,端口1883
  user: mqtt
  password: mqtt
  client_id: zigbee2mqtt2
```

网关适配器/serial:
```shell
serial:
  adapter: ezsp
  port: tcp://[Gateway_IP]:[Port]
 #多模和企业版端口8888 多模自动版端口6638
 #多模自动版域名: port: tcp://tube-zb-gw-efr32-xxxxxx.local:6638 
```

信道/channel:

信道要岔开，防止干扰
```shell
advanced:
  channel: 11
  #信道要分开 选15 20 25
  #z2m网页UI设置步骤z2m设置→高级→ZigBee channel
```
