# Ethos-GPS-Map-Generator
The Ethos GPS Map Generator is a high-precision, web-based tool designed specifically for the FrSky ETHOS community. It simplifies the process of creating custom map backgrounds for the GPS telemetry widget. AI was used in the process of creation.

![Map_Generator_web_interface](https://github.com/user-attachments/assets/4d5b6f2b-169f-4db3-ab63-11f214b09331)


🌟 **Key Features**

🎯 **Navigation & Precision**
**Integrated Search Box:** Powered by the Leaflet Geocoder, allowing pilots to find any flying field or RC club globally by name or address.

**Live Mouse Telemetry:** Displays precision latitude and longitude coordinates in real-time as you move the mouse over the map for pinpoint location checks.

**Center Crosshair:** Provides a permanent visual reference for the exact center of your map, making framing effortless.

🔒 **Control & Framing**
**Hardware-Specific Resolutions:** One-click toggles for 800x480 (Tandem X20 and some of X18 series) and 480x320 (X18 series) to ensure the map fills the radio screen perfectly.

**Precision Zoom Lock:** A specialized safety feature that freezes the map scale. This allows you to pan and center your field without accidentally changing the zoom level, keeping your metadata accurate.

🗺️ **Visual Customization**
**Triple Map Layers:** Choose between Google Hybrid (Satellite with road/location labels), Satellite Only (Clean photo), or Terrain (Topographic contours).

**High-Contrast UI:** Designed with a dark "Stealth" theme to make map details pop, even when using the tool outdoors at the field.

💾 **Intelligent Export System**
**Smart File Naming:** Automatically generates filenames containing the Project Title, the Zoom Scale, and a Timestamp to keep your map library organized.

**Dual-File Export:** Generates the high-quality 24-bit BMP source image and a companion Metadata text file simultaneously.

**Optimized Metadata:** The metadata is pre-calculated with the specific coordinate alignment required by ETHOS hardware, including both DMS (Degrees, Minutes, Seconds) and Decimal formats.

## 🛰️ Metadata Structure
The generated `_metadata.txt` includes:
- **DMS Coordinates:** Degrees, Minutes, Seconds for manual entry. It is MANDATORY to enter them when configuring the GPS map widget.
- **Decimal Geodata:** Precisely formatted North/South/West/East values for the GPS Widget.

📖 **How to Use**

**Download the Ethos-GPS-Map-Generator-main.zip file** and extract it to your local storage. Keep all the files in one folder. Double-click on index.html to open the Ethos GPS Map Generator in your browser.

**Locate:** Use the SEARCH box to find your flying site.

**Frame:** Adjust the zoom level until your flying area is centered in the crosshair.

**Lock:** Check the Zoom Lock box and enter your Project Title.

**Download:** Click ⚡ Export All. You will receive two files - .bmp and _metadata.txt

**Finalize:** 

* **Open Ethos Suite and use the Image Manager to transcode the BMP** to the radio's native 16-bit format.

* Copy the resulting file to your radio SD card path: /Bitmaps/GPS/.

* Use the values in the generated _metadata.txt to configure your GPS widget fields.

![Coordinates_Ethos](https://github.com/user-attachments/assets/35171816-a20f-4991-b2a8-8ef600715bb8)

![Map_accuracy](https://github.com/user-attachments/assets/5ec89c74-d227-4e19-910d-f94d4404befb)

🛠️**Tips for quick access to the coordinates of your flying field**

Your Tandem radio can read .txt documents. To do this, create a Documents folder in the root of the Radio storage (or SD card). Create a User subfolder where you will place all the _metadata.txt files for all the map .bmp files you will be using. This way, you will always have quick access to the coordinates of all the fields you fly to.

RADIO:/documents/user

![File manager](https://github.com/user-attachments/assets/14256bb3-ecc8-41fa-9f13-2e8cc469b153)

![TXT document reading from the radio](https://github.com/user-attachments/assets/ee8009ff-7dd1-4cce-8790-ab8a2c7e3ae2)


