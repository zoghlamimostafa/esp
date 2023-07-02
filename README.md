# ESP32-CAM Web Server

This project demonstrates how to set up an ESP32-CAM module as a web server to capture and serve JPEG images. It uses the `esp32cam` library along with the `WebServer` library to handle HTTP requests and interact with the camera module.

## Table of Contents
- [Requirements](#requirements)
- [Setup](#setup)
- [Usage](#usage)
- [License](#license)

## Requirements

To run this project, you will need the following:

- ESP32-CAM module
- Arduino IDE with ESP32 support
- `WebServer` library
- `esp32cam` library

## Setup

1. Connect the ESP32-CAM module to your computer.
2. Install the required libraries:
   - `WebServer`: Install it from the Arduino Library Manager.
   - `esp32cam`: Download it from the Arduino Library Manager or the library's GitHub repository.
3. Open the `esp32cam_webserver.ino` file in the Arduino IDE.
4. Set the Wi-Fi credentials:
   - Modify the `WIFI_SSID` and `WIFI_PASS` variables in the code to match your network credentials.
5. (Optional) Adjust the IP address configuration:
   - Modify the `local_IP`, `gateway`, and `subnet` variables if you want to set a static IP address.
6. Upload the code to the ESP32-CAM module.
7. Open the Serial Monitor to view the IP address assigned to the module.

## Usage

1. Connect your computer or mobile device to the same Wi-Fi network as the ESP32-CAM module.
2. Open a web browser and enter the IP address shown in the Serial Monitor.
3. The following URLs are available:
   - `/cam-lo.jpg`: Retrieves a low-resolution JPEG image from the camera.
   - `/cam-hi.jpg`: Retrieves a high-resolution JPEG image from the camera.
   - `/cam-mid.jpg`: Retrieves a medium-resolution JPEG image from the camera.
4. Click on the URLs to view the captured images in the browser.
5. You can modify the code to adjust the resolution or other camera settings as needed.

## License

This project is licensed under the [MIT License](LICENSE).
