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

I downloaded firmware to check if it's unzippable. But using `hexeditor` or `ghex` did not help since I was new seeing hexdecimals.

file command shows it's data file.

Used `bchunk` to covert bin and cue to iso worked but could not able to mount on my system.

So I decided to bluetoforce attack using some basic username and password.

then 1 minute late

Found out username and password.

username root

password admin


# some info about CMS7110

`uname -a`

Linux (none) 2.6.17.7 #33 Mon Aug 31 10:44:45 CST 2015 armv5tejl unknown


`cat /proc/version`

Linux version 2.6.17.7 (frankhsu@richwave.buildserver) (gcc version 3.3.4) #33 Mon Aug 31 10:44:45 CST 2015


`cat /proc/meminfo `

MemTotal:        36600 kB

MemFree:          2768 kB

Buffers:         10088 kB

Cached:           2336 kB

SwapCached:          0 kB

Active:          19840 kB

Inactive:        10336 kB

HighTotal:           0 kB

HighFree:            0 kB

LowTotal:        36600 kB

LowFree:          2768 kB

SwapTotal:           0 kB

SwapFree:            0 kB

Dirty:               0 kB

Writeback:           0 kB

Mapped:          19136 kB

Slab:             2008 kB

CommitLimit:     18300 kB

Committed_AS:    26580 kB

PageTables:        464 kB

VmallocTotal:   221184 kB

VmallocUsed:     65652 kB

VmallocChunk:   155132 kB



`cat /proc/cpuinfo`



Processor       : ARM926EJ-Sid(wt) rev 5 (v5l)

BogoMIPS        : 119.60

Features        : swp half fastmult edsp java 

CPU implementer : 0x41

CPU architecture: 5TEJ

CPU variant     : 0x0


CPU part        : 0x926

CPU revision    : 5

Cache type      : write-back

Cache clean     : cp15 c7 ops

Cache lockdown  : format C

Cache format    : Harvard

I size          : 16384

I assoc         : 4

I line length   : 32

I sets          : 128

D size          : 16384

D assoc         : 4

D line length   : 32

D sets          : 128

Hardware        : GUC UMVP-2500

Revision        : 0000

Serial          : 0000000000000000
