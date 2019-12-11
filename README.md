# InstaCrypt
Ransomware for Instagram followers

Ransomware is a type of malware that uses a technique called cryptoviral extortion, in which it encrypts the victim's files, making them inaccessible, and demands a ransom payment to decrypt them. InstaCrypt is a simple ransomware that has only been developed for fun and learning. Instead of asking for money or bitcoins as ransom, this malware demands Instagram followers (Right now the JAR file has my Instagram account linked).

Although the malware application uses simple logic, it seriously encrypts all your files (Size less than 19 MB) in selected directories such as Downloads, Desktop, pictures, etc. The encryption is done using AES with 256-bit key, generated randomly. In order to simplify decryption process, the victim will be in possession of the AES key, encrypted with 2048-bit RSA. The RSA key is hard-coded in the malware application.

The malware generates a random AES key and the encryption process begins. Only after the encryption process is completed, the encrypted AES key file is generated and stored. So, if the process is terminated, intentionally or accidentally, the key file will not be generated and cannot be reproduced again. In this case the encrypted files cannot be decrypted, until AES is broken. The encryption process usually takes some time, and once the entire process is completed, the victim is informed.

I cannot guarantee “reliability” or “security” of the malware application. I am open to criticism, if anyone has any improvements for the cryptographic technique or general implementation, feel free to submit a pull.

Decrypter will soon be added along with various descriptions
There will be no User Interface for Decryptor atleast for now
