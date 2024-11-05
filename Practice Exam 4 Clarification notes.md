
* name the key block cipher encryptions
	* AES, DES, IDEA, blowfish
* name the stream ciphers
	* RC4
* what is an IV
	* random or pseudorandom value used in block cipher modes to ensure that identical plaintext blocks produce different ciphertexts
What is XOR
	"exclusive OR" used for encryption and obsucation
	give definitions for 
	encryptions: transform data into secure format
	obfuscation: make data harder to interpret, not secure it


CBC- chains ciphertext together so each block depends on last
CFB- converts block cipher to stream cipher, allowing encryption of individual bits
CTM combines counter with encryption key to generate stream of pseudorandom data blocks
	adds confidentiality and integrity 

whats the weakest block cipher mode?
	ECB because patterns are visible because identical plaintext blocks encryption identical ciphertexts, so NO IV TO BE FOUND HERE


whats an embedded microcontroller?
	usually a TPM- TPM means trusted platform module

EFS, HSM, FSC, TPM, what are these? - all terms related to *security* like *encrypting* the file  system, managing the keys, encryption in general, and storing keys

EFS: Encrypting file system - WINDOWS feature that ***Asymmetrically*** encrypts files of NTFS volumes

HSM Hardware Security Module - physical device that manages digital keys for strong authentication

FSC- File System Cryptography - general term for encryption at file level

TPM- trusted platform module- secure CHIP for storing encryption keys, supporting secure boot, and verifying system integrity 


PKI, RAS, KDC, NAS, what are these?

PKI- public key infrastructure - managed digital certificates and public key encryption
RAS- Remote Access Service - allows remote network access
NAS - Network Attached Storage - storage device connected to a network for data storage and sharing

Kerberos stuff
KDC- Key Distribution Center - issues session keys for authenticated users

OTP, TGT, AS, TGS
OTP - One Time Password
TGT- Ticket Granting Ticket - kerebos ticket for accessing services
AS Authentication server- kerberos// verifies user identity
whats kerberos

Secure Enclave meaning- part of CPU that is dedicated for sensitive computations (used a lot in Apple products)

steganography?
Hiding data within non-secret data

Tokenization?
	replacing sensitive data with unique identifiers known as tokens to reduce exposure

Data Masking
	Obscures data with characters (eg: credit Card reads "**** **** **** 1957)**
what are hash functions and how do they work?
	Hash functions are algorithms that generate a fixed-size hash from input data

MD5, SHA, CRC, HMAC, what are these and whats the difference between them?

MD5- hash function that is fast and widely used but not secure for crypographic purposes
SHA- family of hash functions with stronger security than MD5
CRC- Cyclic Redundancy check - used for error-checking
HMAC - Hash based message authentication code - Combines Hash with secret key for integrity and authenticity 

block cipher manipulation methods:
* combines unique counter with encryption key to generate a stream of pseudorandom data blocks which are then used for encrypting data
* transforms a block cipher into a stream cipher enabling the encryption of individual bits or bytes of data
* works by chaining ciphertexts blocks together, so each block depends on the previous block