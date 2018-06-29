
# Stream Ciphers

## The One Time Pad

OTP is as long as the message, which is secure & fast but difficult to transfer the key.

## Information Theoretic Security

CT should reveal no 'info' about PT

**perfect secrecy**

## stream ciphers

The time pad is perfect secury based on Shannon, but it is not practitical. So Stream cipher is here to help

idea: replace "random" key by "pseudorandom" key. PRG: is a func G:{0,1}^s --> {0,1}^n, n>>s

PRG must be **unpreditable**
