# 🔥Hashing-Crypto ⤵️
![IMG_7040](https://user-images.githubusercontent.com/94301241/174880818-13e56f93-0825-4a74-af43-cd4382ad0254.jpg)
# 🔑Key Terms 
      Plaintext - Data before encryption or hashing, often text but not always as it could be a photograph or other file instead.
      Encoding - This is NOT a form of encryption, just a form of data representation like base64 or hexadecimal. Immediately reversible.

      Hash - A hash is the output of a hash function. Hashing can also be used as a verb, "to hash", meaning to produce the hash value of some data.

      Brute force - Attacking cryptography by trying every different password or every different key

      Cryptanalysis - Attacking cryptography by finding a weakness in the underlying maths.



# 💥Hash collision URL
      1. https://www.mscs.dal.ca/~selinger/md5collision/
      2. https://shattered.io/
      
# 🧰Automated hash recognition and cracking tools 
      1. hashcat
      2. haiti
      3. hash-identifier
      4. hashid
      4. john the ripper
      
# 🧨Automated hash recognition and cracking tools URL
      1. https://crackstation.net/
      2. https://hashes.com/en/decrypt/hash
      3. https://www.tunnelsup.com/hash-analyzer/
      4. https://md5hashing.net/
      5. https://hashcat.net/wiki/doku.php?id=example_hashes
      
#    👨‍🚒Password Cracking 
     1. Crack this hash: $2a$06$7yoU3Ng8dHTXphAg913cyO6Bjs3K5lBnwq5FJyA6d01pMSrddr1ZG
      Solve: 
            I used https://www.tunnelsup.com/hash-analyzer/ this website this is bcrypt hash.
            In hashcat tool, bcrypt hash code is 3200. You can see this hash code with “hashcat –help” command
            Then I used this command and “rockyou.txt” file for worldlist.
            hashcat -m 3200 <your hash value file> <rockyou.txt file location>
            hashcat -m 3200 hash1.txt /usr/share/wordlists/rockyou.txt
            
      2. Crack this hash: 9eb7ee7f551d2f0ac684981bd1f1e2fa4a37590199636753efe614d4db30e8e1
      Solve:
            I used https://hashes.com/en/decrypt/hash this website to crack this hash value.
      
      3. Crack this hash: $6$GQXVvW4EuM$ehD6jWiMsfNorxy5SINsgdlxmAEl3.yif0/c3NqzGLa0P.S7KRDYjycw5bnYkF5ZtB8wQy8KnskuWQS3Yr1wQ0
      Solve:
            I used https://hashes.com/en/tools/hash_identifier this website this is sha512crypt $6$ hash.
            I saw https://hashcat.net/wiki/doku.php?id=example_hashes this website Sha512crypt mode in hashcat is 1800
            Then I used this command:
            hashcat -m 3200 hash1.txt /usr/share/wordlists/rockyou.txt
      4. Bored of this yet? Crack this hash: b6b0d451bbf6fed658659a9e7e5598fe
      Solve:
            You can use this https://hashes.com/en/decrypt/hash website to crack this hash value.
      
