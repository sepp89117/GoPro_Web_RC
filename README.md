# GoPro_Web_RC
Easily control multiple GoPros with the web browser via Bluetooth, without additional hardware.

GoPro Bluetoothspecs are from https://gopro.github.io/OpenGoPro/ble

<img src="https://github.com/sepp89117/GoPro_Web_RC/blob/main/preview.png" width="630">

Web browsers compatible with Bluetooth API see:
https://developer.mozilla.org/en-US/docs/Web/API/Web_Bluetooth_API#browser_compatibility

# Successfully tested web browsers
- Chrome on PC
- Edge on PC
- Samsung Internet on Android device (App needs permission to search for nearby devices)
- Chrome on Android device (App needs permission to search for nearby devices)

# Successfully tested GoPro models
- Hero 10 Black
- Hero 9 Black
- Hero 8 Black
- Hero 5 Black (load presets not working)

# Number of cameras tested simultaneously
5 Cams

Thanks also to KonradIT for testing!

# How to start
1. Start your GoPro and start pairing with remote
2. Open the Bluetooth manager of your control device (PC, smartphone, etc.) and pair it with "GoPro XXXX". You will then receive a success message on both devices. (The "XXXX" in the name stands for the last 4 digits of the camera serial number)
3. Open "GoPro_Web_RC.html" locally in a supported web browser.
-  Alternatively, the HTML can be hosted over HTTPS. (Web Bluetooth requires TLS)
-  Or browse to https://sepp89117.github.io/GoPro_Web_RC/GoPro_Web_RC.html (thanks @KonradIT)
4. Click on "Connect/Pair new".
5. Your web browser will show you available GoPros. Choose one and click connect.
6. After successful connection, the camera is displayed in the "Connected devices" list.
7. Now you can add more cameras (step 4.) or control the connected cameras.

# TODO
- Check how many cameras it works with at the same time.
- Check which cameras it works with and which don't
- Get all model IDs of known GoPro cameras and assign them the model designation.
- Find commands for Hero 5 load preset
