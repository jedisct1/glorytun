# Glorytun

Small, Simple and Stupid **TCP** VPN.

**Work In Progress:** Do not touch! This code will probably format your harddisk!

Glorytun depends on [libsodium](https://github.com/jedisct1/libsodium) version >= 1.0.4
and needs an AES-NI capable CPU.

To build and install the latest version:

    $ git clone https://github.com/angt/glorytun
    $ cd glorytun
    $ ./autogen.sh
    $ ./configure
    $ make
    # make install

To create and use a new secret key:

    $ hexdump -n 32 /dev/urandom -e '"%X"' > glorytun.key
    # glorytun keyfile glorytun.key [...]
