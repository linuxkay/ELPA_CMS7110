# ELPA_CMS7110
Gained root access to CMS7110. This is some notes step down how to.

# Update

2019/10/03

gained root access.

# Steps I took

First just port scan by anytools

I used nmap though.

The next step is to run fingerprint scan(OS scan) using nmap

`sudo nmap -O targetIP`

Thanks to nmap.

Nmap took little while but told me it's linux 2.6x based system.

I downloaded firmware to check if it's unzippable. But using hexeditor does not help since I was new to using it.

file command shows it's data file.

Used bchunk to covert bin and cue to iso worked but could not able to mount on my system.

So I decided to bluetoforce attack some basic username and password.

then 1 minute late

Found out username and password.

username root

password admin
