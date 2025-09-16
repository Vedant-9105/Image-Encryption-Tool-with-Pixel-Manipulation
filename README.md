PixelCrypt - Web-Based Image Encryption Tool 🖼️🔐
![Technology](https://www.google.com/search?q=https://img.shields.io/badge/tech-HTML | CSS | JS-yellowgreen)

PixelCrypt is an interactive, browser-based tool that demonstrates various image encryption techniques using real-time pixel manipulation. Users can upload an image, apply different encryption algorithms, and see the visual transformation instantly.

Live Demo & Screenshots
This project is a front-end application and can be run by simply opening the index.html file in any modern web browser.

Original Image	Processed Image (XOR Encrypted)

Export to Sheets
Features ✨
Interactive UI: A modern and user-friendly interface with a live preview of the original and processed images.

Multiple Encryption Methods:

Pixel Manipulation: Swap pixel values, invert colors, and shift RGB values.

Mathematical Operations: Apply Addition, Multiplication, or XOR operations to pixel data.

Advanced Techniques: Shuffle entire rows or columns of pixels.

Adjustable Encryption Key: A slider allows users to change the numeric key to vary the encryption strength and output.

Client-Side Processing: All image processing is done in the user's browser using JavaScript and the HTML Canvas API. No server is needed.

Image Upload & Download: Supports drag-and-drop or click-to-upload for images, and allows downloading of both original and processed images.

How It Works 🧠
PixelCrypt leverages the HTML Canvas API to access and manipulate the raw pixel data of an uploaded image.

Image Loading: When a user uploads an image, it is drawn onto a hidden <canvas> element.

Pixel Data Extraction: The canvas's getImageData() method is used to get a Uint8ClampedArray containing the RGBA (Red, Green, Blue, Alpha) values for every pixel in the image.

Manipulation: A selected JavaScript function iterates through this array and modifies the R, G, and B values based on the chosen algorithm and the encryption key. For example:

Invert Colors: new_value = 255 - old_value

XOR Operation: new_value = old_value ^ key

Displaying the Result: The modified pixel data is put back onto a visible canvas using putImageData(), and this canvas is rendered as the "Processed Image". The process is fully reversible if the correct key and inverse operation are applied.

Technology Stack
HTML5: Structures the web application.

CSS3: Provides modern styling, including gradients, flexbox layouts, and a responsive design.

JavaScript (ES6): Powers all the client-side logic, from file handling and UI interaction to the core image processing algorithms via the Canvas API.

How to Run Locally 🚀
No complex setup is required!

Clone the repository or download the files:

Bash

git clone https://github.com/your-username/PixelCrypt.git
Navigate to the project directory:

Bash

cd PixelCrypt
Open the index.html file in your favorite web browser (like Chrome, Firefox, or Edge).

That's it! The application is now running locally on your machine.

License 📄
This project is licensed under the MIT License. See the LICENSE file for details.
