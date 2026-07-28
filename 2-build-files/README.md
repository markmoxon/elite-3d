# Build files for the 6502 Second Processor version of Elite

This folder contains support scripts for building the 6502 Second Processor version of Elite.

* [crc32.py](crc32.py) calculates checksums during the verify stage and compares the results with the relevant binaries in the [4-reference-binaries](../4-reference-binaries) folder

* [elite-checksum.py](elite-checksum.py) adds checksums and encryption to the assembled output

* [elite-decrypt.py](elite-decrypt.py) decrypts an encrypted game binary by doing the opposite to the elite-checksum.py script (this is not used in the build process, but is useful when trying to decrypt any new releases that might be found)

* [DIALG3D.txt](DIALG3D.txt) is a BASIC program by Michael Fairbank that extends the DIALGEN program from the original BBC Micro cassette source discs to draw anaglyph 3D scanner ellipses at various parallax levels, for inclusion in Elite 3D

* [elite-image-whitener.py](elite-image-whitener.py) creates all-white 3D versions of the dashboard and loading screen images, and merges the four anaglyph 3D scanner ellipse images produced by DIALG3D with the all-white dashboard dials in the [images](../1-source-files/images) folder to create the game's 3D dashboards

It also contains the `make.exe` executable for Windows, plus the required DLL files.

---

Right on, Commanders!

_Mark Moxon_