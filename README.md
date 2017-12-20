# ByteChat
## About
### What does ByteChat seek to accomplish?
ByteChat tries to build an ultra-efficient, cryptographically sound and decentralized chat client with a usable UI which will address the following issues:
The dependence on a trusted CA in most of today’s popular secure messaging applications (Telegram, WhatsApp, e.t.c.) which could be known to a government-funded attacker
The inefficiency of protocols and reliance on unsound cryptographic practices


### What is the crypto behind ByteChat?
ByteChat uses LWE and DH key exchange to communicate the two different parts of a key* (LWE is used for early post-quantum support and DH as a fallback in case LWE turns out to be (as the newer option) insecure - plus the attacker would need to have broken both to obtain the key given that the two components are sufficiently random). The key exchange uses a F2F network for public key cryptography but also falls back on a CA mechanism before a proper network of friends is built (these configurations can be changed). Optionally an in-person key exchange (with QR codes) can be used.

### Is ByteChat going to be open-source, can I help?
Help is very welcome, and really the best way to help is to host a ByteChat server (it is as simple as getting a DigitalOcean VPS for about $5/Mo and installing the software found [here](github.com/samuel-allan/ByteChat-Server)) and ByteChat will be open-source and free, the only component that requires hiding will be the CA keys used on the preliminary stages for increased compatibility. Donations are by no means whatsoever expected or required, but if you are very overwhelmingly generous (again - this is purely if you want to make my day) then you can help fund this project: 3BGbbeq3wRfJLP1januueWYYAmuY6jjk6Y (Bitcoin address)

*) **In reality the two parts are exclusive-ored (the security of this given randomness of both components can be easily demonstrated)**

## Installation/Usage
In the future it is assumed ByteChat will be available in all the major software reponsitories on phones (in other words Play store, App store, Windows store). For now the best you can do is contribute and wait :D
