# SSH

- connecting to server; can connect remotely;
- ssh {user}@{host}

rsync -av . root@167.99.146.57:~/super

## how SSH works

Symmetrical Encryption : same key to sender,receiver; KeyExchangeAlgo helps

Asymmetrical Encryption : publicKey, privateKey are linked; thing encrypted by publicKey can only be decrypted by privateKey

@ Diffie-Hellman KeyExchange :

Hashing : String->randomString; MAC

