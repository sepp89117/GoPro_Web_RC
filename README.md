# GoPro_Web_RC
Control multiple GoPros in your web browser

<img src="https://github.com/sepp89117/GoPro_Web_RC/blob/main/preview.png" width="630">

Web browsers compatible with Bluetooth API see:
https://developer.mozilla.org/en-US/docs/Web/API/Web_Bluetooth_API#browser_compatibility

# Successfully tested GoPro models
- Hero 8 Black

# How to start
1. Start your GoPro and start pairing with remote
2. Open the Bluetooth manager of your control device (PC, smartphone, etc.) and pair it with "GoPro XXXX". You will then receive a success message on both devices. (The "XXXX" in the name stands for the last 4 digits of the camera serial number)
3. Open "GoPro_Web_RC.html" locally in a supported web browser. Alternatively, the HTML can be hosted over HTTPS. (Web Bluetooth requires TLS)
4. Click on "Connect/Pair new".
5. Your web browser will show you available GoPros. Choose one and click connect.
6. After successful connection, the camera is displayed in the "Connected devices" list.
7. Now you can add more cameras (step 4.) or control the connected cameras.

# TODO
- Check if it works with multiple cameras and with how many
- Check which cameras it works with and which don't
- Get all model IDs of known GoPro cameras and assign them the model designation. (in readValue() -> case characteristic.uuid == modelNoUUID)
- Get the current mode of the camera via BLE
- Get bluetooth RSSI of camera
