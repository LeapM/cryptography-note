## Course Overview
course includes part1 and part2. Part2 will cover zeor-knowledge, privacy merchanism and other forms of encryption
## addtional resources
[Background on discrete probaility](https://en.wikibooks.org/wiki/High_School_Mathematics_Extensions/Discrete_Probability)

[A course in applied cryptography](http://toc.cryptobook.us/)

[computional number theory](http://shoup.net/ntb/ntb-v2.pdf)

## Objectives

* how crypto primitives work
* use them correclty and reaosn about security

## secuirty communication by SSL/TLS

### objective
* no eavesdropping
* no tampering
### two main steps
1. handshaking stage by using public key cryptography to established a shared secret
2. communicating by using the shared secret

## protect file on disk

### objective
same as commuction no **eavesdropping** and **tampering**

## sym encrytion
E(K,M) := C D(K,C) := M
**NEVER USE A PROPRIETARY CIPHER**

* single use key 
* multi use key

## crypto core
* create shared secret
* secure communication

## what crypto can do

* secure communication
* digital signature
* anonumous communication (mix net by serious of proxies)
* anonymous digital cash (how to prevent double spending) if Alice spent the coin once, no one know. If she spent it twice, everyone know
* secure mutliple party computation (anything can down with trusted auth can also be done without)
* privately outsourcing computation(crypto magic)
* zero knowledge

## rigorous science

* specify threat model
* propose construciotn
* provoe the breaking willl solve an underlying hard problem

## historic example

* substitution cipher. K is an association table. |KEY| = !26. can be break easily by frequency of English letters(e, t, a), frequency of pairs of letters (he, an, in ,th) **cyber text only attack terrible**
  * caesar cipher (shift by N)
* Vigener cipher (16 DC) E = (select a word, repeatedly add to the message, mod 26) D = (M - K ?+26)
assume that we know the length, then use the same frequency cracking techniq as substitution cipher. if we don't know the length of the key, just loop length = 1 to N
* Rotor Machine (*enigma* world war two)
* digital era. Data Encryption Standard(DES), Advanced Encrytion Standard(AES), Salsa20(2008)
  * DES key = 2^56 blocksize = 64 bits
  * AES key = 2^128
