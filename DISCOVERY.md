# Amethyst Protocol Discovery

To let the client know that a given server supports
the Amethyst Protocol the server needs to modify.
The server needs to adjust its 2nd motd line (often called the server description).

The magic sequence:
``0xc2, 0xa7, 0x41, 0xc2, 0xa7, 0x4d, 0xc2, 0xa7, 0x45, 0xc2, 0xa7, 0x54, 0xc2, 0xa7, 0x48, 0xc2, 0xa7, 0x59, 0xc2, 0xa7, 0x53, 0xc2, 0xa7, 0x54``,
needs to be added to the end of the 2nd motd line.

That will cause the client to see that the amethyst protocol is supported.

The next Part is the [Handshake](HANDSHAKE.md).