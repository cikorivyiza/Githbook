# Using ssh Keys



### Steps

1. **ssh-keygen** : creates a pair of keys (Priv+Publ)
2. **ssh-copy-id 192.168.1.10** : copy the public key to the remote server
3. **ssh 192.168.1.10 : you will be able to login without password**
4. **scp /etc/hosts 192.168.4.80:/tmp** : secure copy of the file **hosts** to the remote server in the folder **tmp**
5. **scp 192.168.4.80:/tmp/hosts ./myhosts** :   copying the file hosts from the remote server to my local computer

