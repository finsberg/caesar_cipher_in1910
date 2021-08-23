# Learn testing using Caesar Cipher

In this repo we implement a simple Caesar Cipher algorithm and test some functionality. For more info on how the Caesar Cipher is working check out [Wikipedia](https://en.wikipedia.org/wiki/Caesar_cipher)

## Install
You need python3. No additional packages are required

## Usage
Select a secret key, i.e a shift.

### Encryption
```python
import caesar_cipher
secret_shift = 5
message = "hello"
encypted_message = caesar_cipher.encrypt(message, shift=secret_shift)
```

### Decryption
```python
import caesar_cipher
secret_shift = 5
message = caesar_cipher.decrypt(decrypted_message, shift=secret_shift)
```

## Automated tests
You can run the tests using `pytest`
```
python -m pytest test_caesar_cipher.py
```

## Limitations
This code has quite a lot of limitations
- It only support letters and all letters are converted to lower case. This mean that you cannot encrypt / decrypt messages containing numbers or special characters
- You can only encrypt / decrypt single word, not sentences

## Contributing
Contributions are welcomed, see [CONTRIBUTING.md](CONTRIBUTING.md) for more info
