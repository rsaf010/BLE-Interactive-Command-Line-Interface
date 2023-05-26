# BLE-Interactive-Command-Line-Interface
The BLE Interactive Command Line Interface demonstrates how to control a BLE application using a command line interface. A set of generic BLE commands is provided. The application can be connected to several peripheral and central devices and interact with them. Dynamic subcommands are used to select a peer to interact with based on its BLE device address.

# Setup
Testing the example application requires other BLE devices such as a second nRF5 Development Kit, a smartphone, or other devices. If you want to use the NFC tag reader functionality, enable the sdk_config setting ADAFRUIT_SHIELD. Additional hardware is required for reading NFC tags: Adafruit NFC Shield library.

# BLE Commands
The application BLE commands are organized in a tree structure.

  Root Commands
- advertise           - Turn advertising on or off.
- bonded_devices      - List bonded_devices.
- connect             - <address/peer_id> Establish a connection with a device.
- connected_devices   - Display connected devices and security information on each connection.
- device_name         - <name> Set device name.
- devices             - List available (advertising) devices.
- disconnect          - <address> Disconnect from a device.
- gatt                - GATT Client procedures.
- key_reply           - <key> Enter passkey displayed by another device (for pairing mode: "Passkey Entry").
- nfc_read            - <subcmd> Turn on NFC reader (requires additional hardware) <on/off>.
- numeric             - Confirm or reject a numerical value (for pairing mode: "Numerical Comparison").
- pair                - <subcmd> <address> <option> Initiate pairing with a connected device.
- parameters          - <subcmd> Change or request new Link Layer or GATT parameters.
- privacy             - Set privacy settings.
- remove_bond         - <subcmd> Remove a bonded device.
- scan                - Turn scanning on or off.
- secu                - <LESC/Legacy> choose the security pairing mode
- capability          - <I/O capability> choose the I/O capability to use
  
# 
this app is based on BLE Interactive Command Line Interface Example of Nordic Semiconductor, please refer to the doc for more information about how to use this app with an nrf52 dev kit 
  https://infocenter.nordicsemi.com/index.jsp?topic=%2Fstruct_sdk%2Fstruct%2Fsdk_nrf5_latest.html
