# AES Encryption

128-bit AES Encryption (Rijndael cipher) implemented using x86 assembly.


## Dependancies
All you need is `make` and `nasm`.

Install them using your package manager. 
#### Ubuntu and its derivatives
``` # apt-get update && apt install nasm make```
#### Arch Linux
``` # pacman -S nasm make```

## Steps to run
- Clone this repo.
- Run ```make``` to build the and link the program.	
- Run the executable using ```./AES-Encryption```.
- You can also run the executable as a server. To do so, run the executable with the port as an argument.
	- ```./AES-Encryption 9001```
	- This feature is a WIP.

## How to use

The program has 2 modes, encryption and decryption.
- When encrypting, you just need to give it the key and the message as 16 byte long ascii strings.
	- You will get the encrypted message as a 4x4 matrix.
	- Ex: 
	
		0x4C 0x46 0x9F 0xB6
		
		0x2D 0x7A 0x9B 0x90 
		
		0xB7 0xDF 0xFC 0xB3
		
		0x28 0xA5 0x15 0x3A

- When decrypting, you have to give it the 16 bytes you were given as the encrypted message and the key. The encrypted message is given as 16 2-digit hex bytes, using lowercase characters for a-f.

## More info on AES

- [AES Explained (Advanced Encryption Standard) - Computerphile](https://youtu.be/O4xNJsjtN6E)
- [AES Rijndael Cipher explained as a Flash animation](https://youtu.be/gP4PqVGudtg)
