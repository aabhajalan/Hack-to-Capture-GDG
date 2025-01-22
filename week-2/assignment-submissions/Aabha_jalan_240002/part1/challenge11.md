1) changed the filename to secret.7z after using the file command to check the file type
2) when tried extracting the 7z file, it asked for a password
3) used john the ripper to find the password using the rockyou worlist
    `/usr/share/john/7z2john.pl secret.7z hash.txt`
    `john --format=7z --wordlist=/usr/share/wordlists/rockyou.txt hash.txt`
4) password: `12345abc`
5) used this to extract the hidden file uisng command
    `7z x secret.7z`
6) got a flag(81).txt file, that was a MIME entity. it had a bmp image encoded in base64.
7) copied the base64 text to a new file, named hidden.txt and removed non base64 characters using:
    `sed 's/[^A-Za-z0-9+\/=]//g' hidden.txt > cleaned.txt`
8) deocded the base64 and stored it as a bmp file
    `base64 --decode cleaned.txt > decoded.bmp`
9) `flag: fastctf{the hashcat goes meow}`
