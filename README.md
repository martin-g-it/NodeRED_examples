# NodeRED_examples
NodeRED Examples

ZigBee2MQTT - Aqara Remote vs. IKEA lights
- Switch IKEA lights with the Aqara Remote

Zigbee2MQTT - Color temperature with IKEA E1743
- Change color temperature with a IKEA E1743 on/off switch
- Requires palette: node-red-contrib-counter
- Assumes the remote is binded to the room (means on/off and dimming are not required to be configured
- Clicking the ON button twice within 2 seconds will change color temperature from Cold > Normal > Warm > Cold > etc..

Zigbee2MQTT - Availability - Telegram
- NodeRED flow to send a Telegram message when a Zigbee device gets an 'Availability' timeout.
- Especially helpful for non-pingable devices (e.g. battery powered devices) to raise an alert when the device didn't give any updates in 25 hrs.
- More information on the 'Availability' feature and its settings in Zigbee2MQTT:
  https://www.zigbee2mqtt.io/information/availability.html
- For configuration; see node: README in the flow
- NodeRED pallets required:
    node-red-contrib-telegrambot
    node-red-contrib-counter
