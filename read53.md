# Reading 18:Cryptography

# Encryption, decryption, and cracking 

# Caesar Cipher: invented by Julius Caesar,and One of the earliest encryption techniques, more than two thousand years ago.

# Encrypting a message: 
simple substitution cipher which replaces each original letter with a different letter in the alphabet by shifting the alphabet by a certain amount

# Decrypting a message
Caesar always used a shift of 3. As long as the recipient knew the shift amount, it was trivial to decode the message.

# Cracking the cipher: 

Frequency Analysis
Known plaintext
Brute force


The encryption steps performed are often incorporated as part of more complex schemes, such as the Vigenère cipher. As with all single-alphabet substitution ciphers, the Caesar cipher is easily broken and in modern practice offers essentially no communications security.

# Breaking Cipher:

        The Caesar cipher can be broken even in a ciphertext-only scenario. Two situations can be considered:

        1- an attacker knows (or guesses) that some sort of simple substitution cipher has been used, but not specifically that it is a Caesar scheme.
        2-an attacker knows that a Caesar cipher is in use, but does not know the shift value.
        