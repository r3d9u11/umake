# umake
universal makefile, produced to be easy for usage :)

#### Config Files:
* mk_include.list - set of direcotries to include
* mk_source.list - set of directories with sources
* mk_pkg.list - set of packages from pkg-config to include
* mk_prebuild.list - set of directories with makefile, which should be run within `build` target before main building
* mk_postbuild.list - set of directories with makefile, which should be run within `build` target after main building
* mk_clean.list - set of directories withe makefile, which should be run within `clean` target

#### Variables:
* APPNAME (by default `main`)
* APPEXT (by default for windows `.exe` and empty for linux)
* TARGETOS (values: `windows`, `linux`; by default `autodetection`)
* TARGETARCH (values: `x86`, `x86_64`, `arm`)
* DBGBINDIR (by default `../bin/debug`)
* DBGOBJDIR (by default `../obj/debug`)
* RELBINDIR (by default `../bin/release`)
* RELOBJDIR (by default `../obj/release`)
* SRCEXT (by default `c`)
* MK_SOURCE (by default `../umake-conf/mk_source.list`)
* MK_INCLUDE (by default `../umake-conf/mk_include.list`)
* MK_PKG (by default `../umake-conf/mk_pkg.list`)
* MK_PREMAKE (by default `../umake-conf/mk_prebuild.list`)
* MK_POSTMAKE (by default `../umake-conf/mk_postbuild.list`)
* CC (by default `gcc`)

#### ToDo:
* Add support for shared (dynamic) libraries
  * Build
  * Link
* Add support for static libraries
  * Build
  * Link