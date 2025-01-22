exiftool, steghide, zsteg give nothing
used command
`binwalk --dd=".*" 1.png`
`binwalk --dd=".*" 3.png`
got some files, used hexed.it to figure out which were png files. changed the extension of those.
got two images, used stegsolve to combine the images and get the flag
`flag: CTFlearn{Santa_1s_C0ming}`