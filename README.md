This project is a representation of cryptographic methods. 
Specifically, this is an encryption schema involving key generation, sending, and receiving using Python.
The programs are capable of asymmetric padding and hashing using hmac.


A key pair can be generated and saved in PEM format. Then the sender.py file allows the user to generate a message, which in this case is hardcoded,
"According to all known laws of aviation, there is no way a bee should be able to fly."
Once they are ready to test the strength and efficacy of the encryption, they can being the decryption process using receiver.py.
This will load the reciever's RSA key from the previously created PEM private key. This allows reading from the JSON file.
Using the RSA private key, the AES key can be decrypted based on the SHA256 method.
The MAC is verified and if deemed successful, padding is removed, and the original plaintext message is revealed and outputted.
This receiver.py works functionally the same as the previous sender.py, in reverse.

Run generate.py in command line followed by sender.py and receiver.py
