Epson TM-T20II for Centos8x86_64
=====

Requirenments
=====
* Samba installed.
* Cups installed.
* Cmake dependency installed.

CUPS filter for thermal printer Epson TM-T20II

The linux driver provided on Epson site unfortunately doesn't work.

Filter is provided as src (you can found a list of packages need to be installed in order to build it in the header of source).
Also, printing of blank lines is optimized.

In order to re-compile the binary (e.g. on a Raspberry Pi), the following libraries must be installed:

```
sudo dnf install https://vault.centos.org/centos/8/AppStream/x86_64/os/Packages/cups-devel-2.2.6-40.el8.x86_64.rpm
```

After that, `make` and `./install` do the right thing.
