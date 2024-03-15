# PRODIGY_CS_01

def encrypt(text, shift):
    text = text.lower()
    encrypted_text= ""
    for char in text:
        if char.islower():
            encrypted_text += chr((ord(char) + shift - 97) % 26 + 97)
        else:
            encrypted_text += char
        return encrypted_text

originalMessage = "Prodigy InfoTech Intership 420 60 !!!"
encryptedMessage = encrypt(originalMessage, 2)
print(encryptedMessage)


Output :- rtqfkia kphqvgej kpvgtpujkr 420 60 !!!
