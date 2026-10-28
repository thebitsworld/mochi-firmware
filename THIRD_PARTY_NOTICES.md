# Third-party notices

Mochi firmware (see `LICENSE`) includes the following third-party components. Each is used under its
own license; copies of the license texts are in the `licenses/` folder. These notices apply to the
compiled firmware published at https://github.com/thebitsworld/mochi-firmware as well.

| Component | Copyright | License (file) |
|---|---|---|
| ESP-IDF (Espressif IoT Development Framework), incl. Wi-Fi / BLE / ESP-NOW drivers | Espressif Systems (Shanghai) Co., Ltd. | Apache-2.0 (`Apache-2.0.txt`) |
| FreeRTOS kernel (bundled in ESP-IDF) | Amazon.com, Inc. or its affiliates | MIT |
| lwIP TCP/IP stack (bundled in ESP-IDF) | Swedish Institute of Computer Science | BSD-3-Clause |
| Mbed TLS (bundled in ESP-IDF) | The Mbed TLS Contributors | Apache-2.0 (`Apache-2.0.txt`) |
| Arduino-ESP32 core 3.x (pioarduino) | Espressif Systems; Arduino contributors | LGPL-2.1 for the Arduino API parts (`LGPL-2.1.txt`), Apache-2.0 for the rest |
| LVGL 9.2.2 | Copyright (c) 2021 LVGL Kft | MIT (`MIT-LVGL.txt`) |
| ArduinoJson 7.2.1 | Copyright (c) 2014-2024, Benoit BLANCHON | MIT (`MIT-ArduinoJson.txt`) |
| esp_littlefs | Copyright 2020 Brian Pugh | MIT (`MIT-esp_littlefs.txt`) |
| littlefs | Copyright (c) 2022, The littlefs authors; Copyright (c) 2017, Arm Limited | BSD-3-Clause (`BSD-3-Clause-littlefs.md`) |
| esp-tflite-micro 1.4.1 (TensorFlow Lite Micro) | Espressif Systems; The TensorFlow Authors | Apache-2.0 (`Apache-2.0.txt`) |
| esp-micro-speech-features 1.2.3 | ESPHome; The TensorFlow Authors | Apache-2.0 (`Apache-2.0.txt`) |
| esp_lcd_st77916, es8311, es7210 drivers (copied into `firmware/src/hal/vendor/`) | Espressif Systems (Shanghai) Co., Ltd. | Apache-2.0 (`Apache-2.0.txt`) |
| minimp3 (copied into `firmware/src/hal/vendor/minimp3/`) | lieff | CC0-1.0 (`CC0-1.0-minimp3.txt`) |
| Montserrat font (converted to LVGL bitmap fonts) | Copyright 2024 The Montserrat.Git Project Authors | SIL OFL 1.1 (`OFL-1.1-Montserrat.txt`) |
| Font Awesome Free 5 symbols (via LVGL built-in symbol font) | Fonticons, Inc. | Fonts: SIL OFL 1.1; icons: CC BY 4.0 (`FontAwesome-Free.txt`) |

The "Hey Mochi" wake-word model was trained by thebitsworld with
[microWakeWord](https://github.com/kahrendt/microWakeWord) (Apache-2.0) and
[piper-sample-generator](https://github.com/rhasspy/piper-sample-generator); the training tools are not
part of the firmware.

## LGPL-2.1 components

Parts of the Arduino-ESP32 core are licensed under the GNU Lesser General Public License version 2.1.
You may modify those parts for your own use and reverse engineer the firmware to the extent needed to
debug such modifications. On request, thebitsworld provides the object files of the Mochi application
needed to relink the firmware with a modified version of the LGPL parts. The source code of the
Arduino-ESP32 core is available at https://github.com/espressif/arduino-esp32 and
https://github.com/pioarduino/platform-espressif32.

## Services

Mochi talks to online services that are not part of the firmware and have their own terms: Google
Gemini API (with the owner's own API key), Open-Meteo, ip-api.com, VnExpress RSS, Vietcombank
exchange rates, ntfy.sh, NTP servers.
