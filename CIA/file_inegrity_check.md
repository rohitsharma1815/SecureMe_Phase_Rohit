# File Integrity Check - Integrity Lab

## Objective
Verify data integrity using `sha256sum`.

## Tools Used
- `sha256sum`

## Steps

1. **Create File**
```bash
echo "Important content" > file.txt
# check intial Hash 
  sha256sum file.txt
#Modify the file
  echo "Hacked!" >> file.txt
#check Hash again\
 sha256sum file.txt
# RESULT 
  the hash changed ,proving tha files's integrity was compromised
 so we can check our files are compromie=sed or not by this tool
