# simple-cipher-encoder-decoder
Shift Cipher Encoder/Decoder
This Python script provides a simple implementation of a Shift Cipher, also known as the Caesar Cipher. The Shift Cipher is a substitution cipher where each letter in the plaintext is shifted a certain number of places down or up the alphabet.

Usage
The script allows the user to encode and decode messages using a shift value. The user is presented with a menu offering the following options:

Encode Message: Enter a message and a shift value to encode the message.
Decode Message: Enter an encoded message and a shift value to decode the message.
Exit: Terminate the program.
Encoding
When encoding a message, the script prompts the user to input the message and the desired shift value. Only English alphabet letters are considered for encoding, and any non-alphabetic characters (such as numbers or punctuation) are ignored. The result is a coded message where each letter is shifted by the specified amount.

Decoding
Decoding is the reverse process. The user inputs an encoded message and the shift value used for encoding. The script then decodes the message and displays the original plaintext.

Restrictions
Input Limitations: Messages should consist only of English alphabet letters; any other characters will result in an error message.
Shift Value: The shift value must be a positive or negative integer.
Example
Consider the following example:

Original Message: "hello123"
Shift Value: 3
Encoded Message: "khoor123"
Decoded Message: "hello123"
This example demonstrates the encoding and decoding of a message using a shift value of 3.

Feel free to explore and use this simple Shift Cipher tool for educational purposes and basic text encryption.
