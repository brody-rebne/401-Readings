## Web Security

### HTTPS

- #### Why?
  - Privacy, Integrity, and Identification
  - ##### Privacy
    - Without HTTPS, third parties can intercept communications between client and server
  - ##### Integrity
    - With this ability to intercept, third parties could also manipulate requests or responses between client and server
  - #### Identification
    - Allows for stronger identification
    - Provides digital signature

- #### How?
  - Encryption
  - ##### Types of algorithms
    - ###### Symmetric
      - Uses a single decrypt key
      - Anyone with the key can decrypt
      - Insecure in that the key must be shared
    - ##### Asymmetric
      - Uses multiple keys
      - Only one key is shared
      - Public key is used to encrypt, while private key is used to decrypt
    - ##### The Handshake
      - Process of verification communication between client and server
      - ###### Steps:
        - Client sends set of options for verification and encryption
        - Server chooses best options from set and replies with certificate and public key
        - Client checks certificate and sends an asymmetrically encrypted pre-master key to server
        - Server decrypts the pre-master key and both parties generate a symmetrical key using the pre-master
