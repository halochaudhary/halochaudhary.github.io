# halochaudhary.github.io
EXPRESS QR CODE GENERATOR
### QR Code Generator using QRCode.js

This project is a QR Code Generator built using HTML, CSS, and JavaScript, leveraging the `QRCode.js` library. The generator provides a user-friendly interface to create customizable QR codes on the fly. The key features of the generator include size selection, text input, advanced options for error correction levels, and color customization.

#### Features:

1. **Size Selection**: Users can select the size of the QR code from predefined options, ranging from 100x100 to 350x350 pixels.
2. **Text Input**: A textarea is provided for users to input the text or URL they want to encode into the QR code.
3. **Advanced Options**: 
    - **Color Customization**: Users can select the color of the QR code using a color picker.
    - **Error Correction Level**: Users can choose the error correction level (Low, Medium, Quartile, High) to ensure the QR code remains scannable even if it is partially damaged.
4. **Generate Button**: A button to generate the QR code based on the selected options and input text.
5. **Copy to Clipboard**: A feature that allows users to copy the QR code URL to the clipboard.
6. **Download QR Code**: Users can download the generated QR code as an image file.

#### Usage:

1. **HTML Structure**: The HTML structure consists of a container with elements for text input, size selection, advanced options, and buttons for generating, copying, and downloading the QR code.
2. **CSS Styling**: Basic styling is applied to ensure a clean and responsive user interface.
3. **JavaScript Functionality**: 
    - The `QRCode.js` library is used to generate the QR codes.
    - The `genQR` function generates the QR code based on user inputs and appends it to the specified container.
    - The `copyToClipboard` and `downloadQR` functions provide additional functionality to copy the QR code URL and download the QR code image, respectively.

#### How It Works:

1. **Include QRCode.js Library**: The library is included via a CDN link:
    ```html
    <script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
    ```
2. **Generate QR Code**: When the user clicks the "Generate QR" button, the `genQR` function is invoked. This function:
    - Retrieves user inputs for text, size, color, and error correction level.
    - Clears any previously generated QR code.
    - Generates a new QR code with the specified parameters using the `QRCode` class from `QRCode.js`.
    - Displays the QR code on the page and shows additional options for copying and downloading.
3. **Copy and Download Functions**: 
    - The `copyToClipboard` function converts the QR code to a Blob URL and copies it to the clipboard.
    - The `downloadQR` function converts the QR code to a PNG image and triggers a download.

This project demonstrates how to create a dynamic and customizable QR code generator using JavaScript and an external library, providing a practical tool for generating QR codes for various purposes.
