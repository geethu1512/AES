# EX-8-ADVANCED-ENCRYPTION-STANDARD ALGORITHM
# Aim:
To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption.

# ALGORITHM:
AES is based on a design principle known as a substitution–permutation.
AES does not use a Feistel network like DES, it uses variant of Rijndael.
It has a fixed block size of 128 bits, and a key size of 128, 192, or 256 bits.
AES operates on a 4 × 4 column-major order array of bytes, termed the state
# PROGRAM:
~~~
def xor_encrypt(text, key):

    result = ""

    for i in range(len(text)):

        ch = chr(ord(text[i]) ^ ord(key[i % len(key)]))

        result += ch

    return result

message = "GEETHU"
key = "secretkey"

print("Original Message:", message)

encrypted = xor_encrypt(message, key)

print("Encrypted Message:", encrypted)

decrypted = xor_encrypt(encrypted, key)

print("Decrypted Message:", decrypted)

print("AES Encryption Program Completed")
~~~
# OUTPUT:
<img width="1371" height="672" alt="AES outpiut" src="https://github.com/user-attachments/assets/7b262268-859d-49f6-ad12-625d3b13dcb6" />


# RESULT:
The AES Encryption algorithm for URL Encryption was implemented successfully.

