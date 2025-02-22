Image Steganography using OpenCV

Description

This Python script performs basic image steganography by hiding a secret message inside an image. The message is stored by modifying pixel values, and it can be retrieved using a correct passcode.

Prerequisites

Ensure you have the following installed:

Python 3.x

OpenCV (cv2)

You can install OpenCV using:

pip install opencv-python

Features

Hide messages inside images using pixel modification.

Retrieve hidden messages with a correct passcode.

Works with standard image formats like JPEG and PNG.

Simple and lightweight implementation with Python and OpenCV.

How It Works

Encryption (Hiding the Message):

The user provides an image (mypic.jpg).

The user enters a secret message and a passcode.

The script modifies pixel values to store the message.

The modified image is saved as encryptedImage.jpg.

Decryption (Retrieving the Message):

The user enters a passcode.

If the passcode matches, the script extracts and prints the hidden message.

If the passcode is incorrect, access is denied.

Usage

Encrypt a Message

Ensure you have OpenCV installed and an image file ready.

Run the script in your Python environment.

Input the secret message and passcode when prompted.

The encrypted image (encryptedImage.jpg) will be saved automatically.

Decrypt a Message

Run the script again.

Enter the passcode used during encryption.

If correct, the hidden message will be revealed.

Known Issues

The script modifies pixel values directly, which can distort the image.

The message length must not exceed the number of available pixels.

The current method of storing data isn't robust; improvements are needed to avoid loss of information.

Future Improvements

Use a more systematic approach for encoding (e.g., LSB steganography).

Implement a method to track message length and prevent errors.

Add error handling for incorrect inputs and missing files.

Contribution

Contributions are welcome! If you'd like to improve this project, feel free to fork the repository, make modifications, and submit a pull request. You can also report issues or suggest enhancements via the issue tracker.

