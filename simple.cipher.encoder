def shift_cipher(message, shift):
    result = ""
    for char in message:
        # Check if the character is a letter and determine its case.
        if char.isalpha():
            # Shift the letter and wrap around when reaching the end of the alphabet.
            result += chr((ord(char) - ord('a' if char.islower() else 'A') + shift) % 26 + ord('a' if char.islower() else 'A'))
        else:
            # If the character is not a letter, display an error message.
            print("Invalid input. The message should consist only of English alphabet letters.")
            return None
    return result

def encode_message():
    print("\n--- Message Encoding ---")
    # Display a warning message to the user.
    print("Please use only English alphabet letters. Do not use Turkish characters, numbers, or punctuation.")

    # Get the message and shift value from the user for encoding.
    message = input("Enter a message to encode: ")

    # If the user enters invalid input, terminate the encode_message function.
    for char in message:
        if not char.isalpha() or (char.isalpha() and not char.isascii()):
            print("Invalid input. The message should consist only of English alphabet letters.")
            return

    shift = int(input("Enter the shift value: "))
    encoded_message = shift_cipher(message, shift)
    if encoded_message is not None:
        # Encode the message and print the result.
        print("\nEncoded Message:", encoded_message)

def decode_message():
    print("\n--- Message Decoding ---")
    # Display a warning message to the user.
    print("Please use only English alphabet letters. Do not use Turkish characters, numbers, or punctuation.")

    # Get the encoded message and shift value from the user for decoding.
    message = input("Enter a message to decode: ")

    # If the user enters invalid input, terminate the decode_message function.
    for char in message:
        if not char.isalpha() or (char.isalpha() and not char.isascii()):
            print("Invalid input. The message should consist only of English alphabet letters.")
            return

    shift = int(input("Enter the shift value: "))
    decoded_message = shift_cipher(message, -shift)
    if decoded_message is not None:
        # Decode the message and print the result.
        print("\nDecoded Message:", decoded_message)

def main():
    while True:
        print("\n╔══════════════════════════════════╗")
        print("║             - MENU -             ║")
        print("╠══════════════════════════════════╣")
        print("║ 1. Select to Encode a Message    ║")
        print("║ 2. Select to Decode a Message    ║")
        print("║ 3. Exit                          ║")
        print("╚══════════════════════════════════╝")

        # Get the user's choice.
        choice = input("Please select (1/2/3): ")

        if choice == '1':
            encode_message()
        elif choice == '2':
            decode_message()
        elif choice == '3':
            print("\nExiting the program.")
            break
        else:
            print("\nInvalid input. Please enter 1, 2, or 3.")

if __name__ == "__main__":
    main()

