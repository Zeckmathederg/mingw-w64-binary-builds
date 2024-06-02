# mingw-w64-binary-builds
Mingw-w64 binary builds to help users bootstrap a mingw-w64 toolchain
for their system! Ideal for Linux From Scratch and building Wine!
# What to do
Go to the releases section and download the packaged tarball then unpack
it wherever (/opt is recommended)! Change the `PATH` variable to be
`$MINGWDIR/usr/bin:$PATH` where `$MINGWDIR` would be replaced with where
you unpacked the mingw-w64 tarball, including the resulting directory
itself. Then you're ready to do what you must to compile binutils,
mingw-w64-{headers,crt,winpthreads}, and finally gcc for the
"$architecture"-w64-mingw32 target to bootstrap the mingw-w64 toolchain!
The resulting files can be put in /usr and you will no longer need to
depend on your binary mingw-w64 installtion provided here to run the
toolchain and compile projects like Wine or software targeting Windows.
For instructions on how to compile that software, start at
https://zeckmathederg.github.io/glfs/wine/mingw-w64-binary.html and go
from there. Stop at libxkbcommon. If you intend to compile Wine on an LFS
system, please read https://zeckmathederg.github.io/glfs from the beginning.
