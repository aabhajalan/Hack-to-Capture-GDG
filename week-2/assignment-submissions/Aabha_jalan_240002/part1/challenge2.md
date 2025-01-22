used commands
`xxd unopenable.gif | head`
`xxd unopenable.gif | tail`
the tail matches the magic number for gif
so changed the head to 
`47 49 46 38 39 61  (GIF89a)`
using hexed.it
the file command shows it as a GIF file.
used the command
`convert unopenable.gif repaired.gif`
got  `ZmxhZ3tnMWZfb3JfajFmfQ==` base-64 encoded string
used command
`echo  ZmxhZ3tnMWZfb3JfajFmfQ== | base64 --decode`
flag: `{g1f_or_j1f}`

