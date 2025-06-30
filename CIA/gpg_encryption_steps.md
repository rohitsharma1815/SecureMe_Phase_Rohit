# GPG Encryption - Confidentiality Lab

## Objective
To demonstrate the use of GPG to encrypt and decrypt files, protecting data confidentiality.

## Tools Used
- `gpg` (GNU Privacy Guard)
- Ubuntu 22.04

## Steps

1. **Install GPG**
```bash
sudo apt update && sudo apt install gnupg
# Create a Test file 
  echo "This is a secret message" > secret.txt
# Generate GPG Key
  gpg --full-generate-key
# Encrpyt File
 gpg -e -r "Your Name" secret.txt
 #Decrpyt File
  gpg -d secret.txt.gpg
  



