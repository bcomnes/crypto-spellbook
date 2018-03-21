# Primitives + Concepts

## Public and private key pairs

## HMAC

- https://en.wikipedia.org/wiki/HMAC

> HMAC does not encrypt the message. Instead, the message (encrypted or not) must be sent alongside the HMAC hash. Parties with the secret key will hash the message again themselves, and if it is authentic, the received and computed hashes will match.

https://github.com/jedisct1/libsodium-doc/issues/12#issuecomment-189775445

> <emilbayes> 11:42 bret: One of application that the BLAKE authors mention in the blake book is that it was designed to be used as a prefix MAC, meaning you supply a secret key (hence the crypto_generichash key parameter) and then hash your file. Another party can then use the same key and do the hashing again and check
11:43 bret: It's called a prefix mac to differentiate it form a HMAC, since that works differently, despite the idea kinda being the same (creating a MAC from a hash function)
11:45 also, the prefix mac is just blake2b(key || data)
