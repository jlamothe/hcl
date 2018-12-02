# HCL Change Log

## current

* added `ChangeLog.md` to cabal file
* `reqCont` catches `IOError` in first `Request`, and falls back to second
* `reqDefault` catches `IOError` and returns the default value

## v1.7

* `reqIO` now catches `IOError` and returns `Nothing`
* implemented `reqLiftMaybe`

## v1.6

* added test suite
* fixed compiler warnings
* documemtation fixes
* defined `Request` as `Alternative` and `MonadPlus`

## v1.5.1

* fixed broken cabal file

## v1.5

* modified code to compile against QuickCheck 2.*
  * made `Request` a `Functor` and `Applicative`
* implemented `reqChar` and `reqPassword`