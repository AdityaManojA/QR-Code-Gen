# 👾 Retro QR Crafter

A web-based utility for bulk generating and scanning QR codes, wrapped in a fun, retro 8-bit theme. Easily convert a list of IDs, texts, or links from an Excel file into individual QR codes, and download them all in a single ZIP file. The built-in scanner can decode QR codes either from an uploaded image or by capturing a new photo with your device's camera.

**Live Demo:** <https://text-based-qr.netlify.app/>

## ✨ Features

* **📦 Bulk QR Code Generation**: Upload an `.xlsx` Excel file to generate QR codes for every entry in the first column.
* **🔗 Text & Link Support**: Works perfectly with plain text, IDs, or web links.
* **💾 Download All**: Compress and download all generated QR codes as a single `.zip` file for easy distribution.
* **📸 Dual-Mode QR Scanner**:
  * **Capture Photo**: Use your device's camera to take a picture of a QR code and scan it.
  * **Upload Image**: Scan a QR code from an existing image file.
* **🔍 Click to Enlarge**: Click on any generated QR code to view a large, high-contrast version for easy scanning.
* **🎮 Retro UI**: Fun and stylish 8-bit, Minecraft-inspired interface with a custom pixel font.
* **🔒 Fully Client-Side**: No data is ever sent to a server. All processing is done securely in your browser.
* **📱 Responsive Design**: Works on both desktop and mobile devices.

## 🚀 How to Use

### Generating QR Codes

1. **Prepare Your Data**: Create a simple `.xlsx` file. Place all the data you want to convert into QR codes in the **first column**. The app ignores all other columns and sheets.
2. **Upload the File**:
   * Navigate to the **Generator** tab.
   * Click "Choose File" and select your `.xlsx` file.
3. **Generate**:
   * Once the file is loaded, click the "Generate Codes" button.
   * All corresponding QR codes will be displayed in a grid.
4. **Download**:
   * Click the "Download All as .ZIP" button to save all the codes to your computer.

### Scanning QR Codes

1. **Navigate to Scanner**: Click the **Scanner** tab.
2. **Choose a Method**:
   * **To Take a Photo**:
     1. Click "Take a Photo".
     2. Grant camera permissions if prompted.
     3. Point your camera at the QR code and click "Capture Photo".
     4. Review the captured image and click "Scan This Photo". You can also "Retake Photo".
   * **To Upload an Image**:
     1. Click "Choose Image".
     2. Select a QR code image file from your device.
3. **View Result**: The decoded text or link will appear in the result box.

## 💻 Technologies Used

* **HTML5, CSS3, JavaScript**: Core web technologies.
* **Tailwind CSS**: For styling the user interface.
* [**SheetJS (xlsx.js)**](https://github.com/SheetJS/sheetjs): To read and parse `.xlsx` files.
* [**QRious**](https://github.com/neocotic/qrious): For generating QR codes.
* [**JSZip**](https://github.com/Stuk/jszip): For creating the `.zip` archive.
* [**FileSaver.js**](https://github.com/eligrey/FileSaver.js/): For saving the generated zip file.
* [**html5-qrcode**](https://github.com/mebjas/html5-qrcode): For handling camera access and QR code scanning.
* **Google Fonts ('Press Start 2P')**: For the retro pixelated font.

## 🛠️ Local Setup

This project is a single `index.html` file with no build steps required.

1. Clone the repository or download the `index.html` file.
2. Open the `index.html` file in any modern web browser.

That's it! The application will be fully functional.
