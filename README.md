# secret-message-encoder-decoder
🔒 Secret Encoder/Decoder by Pratik Mishra
This is a single-file web application designed to demonstrate two key security concepts: Symmetric Encryption (Shift Cipher) and Steganography (Data Hiding).
It allows a user to encrypt a visible message and simultaneously hide a completely separate, secret message within the output string using a unique symbol marker.
✨ Features
• Polyalphabetic Shift Cipher: Encrypts and decrypts the main visible text using a numerical key (0-999).
• Steganography: Hides a secondary message (Base64-encoded for obfuscation) directly inside the encrypted main text.
• Custom Marker: Uses a user-defined symbol or sequence (e.g., 🔑🍎, [SECRET]) to clearly mark where the hidden payload begins.
• Single-File Simplicity: The entire application is contained within one lightweight index.html file (HTML, Tailwind CSS, and pure JavaScript).
🚀 How to Use It
The application requires three crucial pieces of information to encode or decode a message:
1. Shift Key: The main numerical key used to scramble/unscramble the visible text.
2. Hidden Symbol Sequence: The exact marker (e.g., 🔑OK) that separates the encrypted main message from the hidden payload.
3. Input/Output Message: The text to be processed.
Encoding a Secret
1. Enter your Shift Key (e.g., 17).
2. Enter your Hidden Symbol Sequence (e.g., 🔒OK).
3. Enter your Secret Message (this will be hidden).
4. Enter your Input Message (this will be the visible, encrypted text).
5. Click "Encode & Hide Secret" (Blue Button).
6. The result in the Output box will be a long string containing the encrypted text, the symbol sequence, and the Base64 secret payload.
Decoding the Message
1. Set the Shift Key and Hidden Symbol Sequence to the exact values used for encoding.
2. Paste the entire long encrypted string into the Input Message area.
3. Click "Decode & Reveal Secret" (Red Button).
4. The app will instantly display the original main message and reveal the hidden secret in the yellow box.
🛠 Technology Stack
This project is a classic static application with zero dependencies outside of the browser:
• HTML5: Structure.
• Tailwind CSS (via CDN): Modern, responsive styling.
• Pure JavaScript: All logic, including the Shift Cipher, Base64 encoding/decoding, and DOM manipulation.
