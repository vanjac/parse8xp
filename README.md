# Python TI83 BASIC converter

This is a fork. Look at the original repo's README for instructions and more information.

Here's what I'm changing, or in the process of changing:
- Full Python 3 support, no Python 2 support. This isn't complete yet.
- Decompiled programs will now always be ONLY plaintext. The original script used to fill them with null bytes and other things. These files are now written in text mode rather than binary mode, so there no longer has to be support for different line endings, etc.
- I have been checking the script by decompiling a program from my TI-84 and recompiling it, and checking the differences. I found a few differences with the programs the script was generating. Most importantly the checksum calculation was completely incorrect. I've made corrections based on these discrepancies and now, for the few programs I've checked so far, the recompiled programs are identical byte-for-byte.
