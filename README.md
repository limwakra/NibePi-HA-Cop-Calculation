# NibePi-HA-Cop-Calculation
Node-Red Flow in combination with Home Assistant, NibePi Nibe Cop calculation.

Calculation is based on [link](https://github.com/karhulitos/MLPlogintutkija)


## Prerequisites
This tutorial assumes the following:
- A working nibepi connected to your heat pump and reachable on your local network (MQTT HA Dicovery activated)
- A working [mqtt server/broker](https://mqtt.org/). Either in Home Assistant as [add-on (instructions link)](https://github.com/home-assistant/addons/blob/174f8e66d0eaa26f01f528beacbde0bd111b711c/mosquitto/DOCS.md#how-to-use) or stand alone.
- A working [Home Assistant](https://www.home-assistant.io/) system
- [Node-Red](https://community.home-assistant.io/t/home-assistant-community-add-on-node-red/55023) running as an add-on in Home Assistant.
- In Node-Red add [node-red-contrib-ha-mqtt](https://flows.nodered.org/node/node-red-contrib-ha-mqtt) To push the data back to Home Assistant.
- In NibePi activate these in "Datahantering":
  * EB100-EP14-BT3(40012) = BT3
  * EB100-EP14-BT10(40015) = BT10
  * EB100-EP14-BT12(40017) = BT12
  * EB100-EP14-BT14(40018) = BT14
  * EB100-EP14-BT17(40022) = BT17
  * Compressor frequency, Actual (43136)
  * EB100-EP14 PCA Base Relays (43514)
  
<img width="1065" alt="Schermafbeelding 2023-10-22 om 20 48 20" src="https://github.com/limwakra/NibePi-HA-Cop-Calculation/assets/97366516/15ffd6e8-defa-4cb5-8e3e-6d2b66e25e53">
<img width="1279" alt="Schermafbeelding 2023-10-23 om 11 10 20" src="https://github.com/limwakra/NibePi-HA-Cop-Calculation/assets/97366516/1f173c35-80d4-4b94-990c-f82a0ed6fbc3">
