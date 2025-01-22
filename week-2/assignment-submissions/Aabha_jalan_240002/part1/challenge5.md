1) nothing on file, exiftool.
2) saw a RAR file using zsteg command
3) extracted the hidden files using binwalk and then extracted the archive file using online extractor
4) got an audio file and another RAR file, with the header Cat! instead of Rar!.
5) on running the audio file on sonic visualiser, got the text
`sp3ctrum_1s_y0ur_fr13nd`
6) use command `strings <filename>` on the rar file, and found a fin4ally.txt file.
6) when trying to use the unrar command, it shows some error, so repair it using command
` rar r y0u_4r3_cl0s3.rar`
7) use command on the repaired file 
`unrar x rebuilt.y0u_4r3_cl0s3.rar`
8) got a base 64 encoded text
10) `flag: {f0r3n51cs_ma5t3r}`
