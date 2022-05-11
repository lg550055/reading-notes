# Cryptography
The word cryptography comes from Greek kryptos (secret/hidden) and graphein (to write).

- > Encryption: scrambling the data according to a secret key
  - Cipher -an algorithm that converts plain text into Ciphertext
- > Decryption: recovering the original data from scrambled data by using the secret key.
- > Code cracking: uncovering the original data without knowing the secret

> The are four primary types of cryptography in use today, each with its own unique advantages and disadvantages:

- hashing -changes a message into an unreadable string for the purpose of verifying the message’s contents, not hiding the message itself
- symmetric cryptography -single key known to sender and recipient; its primary use is protecting restind data (e.g. databases) and mostly relies on AES*

- asymmetric cryptography -two keys, a public and a private.  One to encypt, but not decrypt;  commonly used in secure interenet communications

- key exchange algorithms -allow sender and recipient to agree on a key without sending one**.  It relies on 'one-way functions', which are mathematical operations that are very easy to do in one direction, but very hard to reverse, e.g., modular exponentiation

* Advanced Encryption Standard (AES) 2001
- Key length 128 - 256 bits
- Chops data into 16-byte blocks
- applies a series of substitutions and permutations based on the key value
- this process is repeated 10+ times for each block
- The longet the key the longer it takes to encrypt and decrypt; AES balances security and performance


** ![Example of key exchange algorithm)](https://thebestvpn.com/wp-content/uploads/2017/06/n4jBE-1.png)

---

### Resources

- [Encryption, Decryption & Hacking](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:online-data-security/xcae6f4a7ff015e7d:data-encryption-techniques/a/encryption-decryption-and-code-cracking)
- [Cryptography Crash Course](https://www.youtube.com/watch?v=jhXCTbFnK8o)
- [Introduction to Cryptography](https://thebestvpn.com/cryptography/)



---

[Back to table of contents](../README.md)