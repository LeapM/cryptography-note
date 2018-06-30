
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

## attach on OTP

### two time pad
never use the stream cipher key more than once C1 xor C2 = M1 xor M2 --> M1 , M2(due to the redundancy in **(English and ASCII)**

real example
* project Venona
* MS-PPTP(windows NT)
* 802.11B WEP suffer from two kind of attached
  * Two time pad attached(RPG(IV || K). IV is 24 bit, after about 2^24, it will recycle, then two time pat attached can occure
  * PGR is RC4, since IV is sequnce number, the IV || K is very similar, which RC4's seed can be recovered after about 40,000 frame
  **how to avoid** treat multiple frames as a long long string, or generate a long long key and use part of the key for each frame
  
### attack 2: no integrity(OTP is malleable)

attacher can modify the text without being identified

## Realworld example

### RC4 is used in HTTPS and WEP

Weekness
1. Bias in initial output Pr{2nd bypte = 0] = 2/256
2. Prob of (0,0) is 1/256^2 + 1/256^3
3. Related key attach happened in WEP

### CSS centent scramming system used in DVD

steam cipher based on linear feedback shift register (LFSR)

* CSS seed = 5 bytes = 40bits(due to the US export law)

### EStream the good one
Estream project has 5 stream cyper

* eStream Salsa 20 (sw+hw)
* Sosemanuk


