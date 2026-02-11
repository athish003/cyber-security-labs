# cyber-security-labs
for learning and documenting the learning process

import hashlib

import hmac

4

5

message = input("Enter the message: ")

key input("Enter the secret key:

").encode()

# Secret key needs to be encoded to bytes

8

9

10

11

12

13

14 15

16

17

hash_object = hashlib.sha256(message.encode())

hash_hex hash_object.hexdigest()

print(f"\nSHA-256 Hash: {hash_hex}")

mac_object = hashlib.pbkdf2_hmac('sha256', message.encode( key, 100000)

mac_hex = mac_object.hex()

print(f"MAC (using SHA-256): (mac_hex}")

hmac_object = hmac.new(key, message.encode(), hashlib.sha256) hmac_hex = hmac_object.hexdigest()

print(f"HMAC (using SHA-256): {hmac_
