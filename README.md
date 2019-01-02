Nix, the purely functional package manager
------------------------------------------

Nix is a new take on package management that is fairly unique. Because of its
purity aspects, a lot of issues found in traditional package managers don't
appear with Nix.

To find out more about the tool, usage and installation instructions, please
read the manual, which is available on the Nix website at
<http://nixos.org/nix/manual>.

## Contributing

Take a look at the [Hacking Section](http://nixos.org/nix/manual/#chap-hacking)
of the manual. It helps you to get started with building Nix from source.

## License

Nix is released under the LGPL v2.1

This product includes software developed by the OpenSSL Project for
use in the [OpenSSL Toolkit](http://www.OpenSSL.org/).


### COMPILING ###

dependancies:
bash
autotools
libtool
pkg-config / pkgconf
openssl
sqlite3
gmake
boost
editline (https://github.com/p01arst0rm/editline)

this source is a little weird; make sure editline is compiled
and installed from source with the parameters:
./configure --prefix=/usr
make SHLIB_LIBS=-lcurses
sudo make install

after installation, be sure to use sudo ldconfig to reload.

make sure to run libtoolize before building all source pkgs
