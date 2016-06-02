# PassLok4email
PassLok for Email is a Chrome extension that adds PassLok encryption to webmail apps. Initially for Gmail only, we are planning to add Yahoo and Outlook very soon.

PassLok for Email is powerful, since it is based on NaCl (tweetNaCl JavaScript version, published here on GitHub), including the 256 bit XSalsa20 symmetric cipher and Curve25519 functions for asymmetric encryption. PassLok for Email also includes the WiseHash variable-strength key derivation algorithm so users are not restricted in their choice of private keys.

PassLok for Email is also designed to be very easy to use. The sender's Lock (public key) is added to every encrypted message, and retrieved automatically on the recipient's end so he/she does not need to bother with key management chores. The only key-management action requested of the user is entering his/her secret Password, from which the private key derives, when the encryption engine is initialized. The private key is retained in memory for five minutes beyond the last use of it and then deleted. It is never stored in any way.

WARNING TO TESTERS: the compression algorithm has changed with verison 0.2.2, so messages encrypted with previous versions decrypt to nothing, though decryption is successful. Hopefully there won't be a need for further changes for a while.


