### v5.0.0 (2025-01-30)

* Renamed to mirage-mtime (from mirage-clock), only the MCLOCK part
* use "dune variants" for the different implementations

### v4.2.0 (2022-03-27)

* Rename the freestanding toolchain to solo5 (@dinosaure, #51)
* Use ocamlformat (@samoht, #54)

### v4.1.0 (2022-02-01)

* Be able to build & instal the distribution via `opam` without the expected `dune`'s context (@TheLortex, @dinosaure, #49)

### v4.0.0 (2021-11-15)

* Remove Mirage_clock_lwt module (#48 @hannesm)
* Use caml_get_wall_clock instead of unix_gettime to avoid floating point
  conversion roundtrip (#47 @hannesm)

### v3.1.0 (2020-11-19)

* Use implicit executable dependency for discover.exe
  into the dune file (#46 @TheLortex)
* Fix cross-compilation on Android (#45 @EduardoRFS)

### v3.0.1 (2019-11-04)

* provide deprecated Mirage_clock_lwt for smooth transition (#44 @hannesm)

### v3.0.0 (2019-10-21)

* remove mirage-clock-lwt (#43 @hannesm)
* mirage-clock is no device anymore, drop lwt dependency (#43 @hannesm)
* raise lower OCaml bound to 4.06.0 (#43 @hannesm)

### v2.0.0 (2018-12-27)

* Constrain the clock type `t` to `unit` to improve compatability with
  the webmachine CLOCK interface. All current implementations satisfy
  this interface so there shouldn't be an issue, but bumping the
  library major version number to reflect the interface change (#38 @hannesm)

* Port library to Dune from jbuilder and use `dune-release` and the builtin
  `dune.configurator` to reduce the build dependency cone (#39 @avsm).

* Remove unused variable warnings (#39 @avsm).

* Update opam package metadata to 2.0 format (#39 @avsm).

* Fixes to the ocamldoc comment headers for odoc compatibility (@avsm)

### v1.4.1 (2018-08-03)

* mirage-clock-unix: fix integer overflow on 32 bit (#37, @mattgray)

### v1.4.0 (2017-07-25)

* Add support for windows to `mirage-clock-unix` (#32, @fdopen and @samoht)

### v1.3.0 (2017-06-19)

* port to Jbuilder

### v1.2.0 (2016-12-21)

* import `V1.MCLOCK` and `V1.PCLOCK` from `mirage-types` under `mirage-clock`
  and `mirage-clock-lwt`

### v1.1.0 (2015-01-05)

* xen: pure OCaml implementation of `Clock.gmtime`

### v1.0.0 (2013-12-07)

* Remove unnecessary cstruct dependency.
* Install ocamlfind packages as `mirage-clock-xen` and `mirage-clock-unix`.
* Fix META file descriptions.
* Add Travis tests.

### v0.9.9 (2013-12-05)

* Initial public release, based on mirage/mirage-platform#0.9.8
