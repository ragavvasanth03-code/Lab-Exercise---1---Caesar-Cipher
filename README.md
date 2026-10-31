# Lab-Exercise---1---Caesar-Cipher
# Aim 
To encrypt and decrypt the given message by using Ceaser Cipher encryption algorithm.
# Procedure 
Step 1: Design of Caeser Cipher algorithnm 
Step 2: Implementation using C or pyhton code Step 3:In Ceaser Cipher each letter in the plaintext is replaced by a letter some fixed number of positions down the alphabet. For example, with a left shift of 3, D would be replaced by A, E would become B, and so on.

Step 3: The encryption can also be represented using modular arithmetic by first transforming the letters into numbers, according to the scheme, A = 0, B = 1, Z = 25. 
Step 4:Encryption of a letter x by a shift n can be described mathematically as, En(x) = (x + n)mod26 
Step 5:1 Decryption is performed similarly, Dn (x)=(x - n) mod26
# Program 
```
message = input("Enter a message: ")
shift = int(input("Enter shift value: "))

result = ""

for ch in message:
    if ch.isupper():
        ch = chr((ord(ch) - ord('A') + shift) % 26 + ord('A'))
    elif ch.islower():
        ch = chr((ord(ch) - ord('a') + shift) % 26 + ord('a'))

    result = result + ch

print("Encrypted message:", result)
```
# output
<img width="1556" height="595" alt="Screenshot 2026-10-26 100206" src="https://github.com/user-attachments/assets/c1e53939-8055-4c3f-9113-a27ccb0f365c" />

# Result
The program is executed successfully.
