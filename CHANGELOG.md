## Unreleased Changes

[Full Changelog](https://github.com/guard/guard-minitest/compare/v1.0.0...master)

Nothing here.

## 1.0.0 - May 8, 2013

[Full Changelog](https://github.com/guard/guard-test/compare/v0.8.0...v1.0.0)

### New feature

- [#40][], [#41][] Add support for running tests via `spring`. ([@pgaertig][])

### Improvements

* Get rid of `autoload`. ([@rymai][])

## 0.8.0 - March 24, 2013

[Full Changelog](https://github.com/guard/guard-test/compare/v0.7.0...v0.8.0)

### New feature

* [#38][] Add support for running tests via `zeus`. ([@djmaze][])

## 0.7.0 - November 6, 2012

[Full Changelog](https://github.com/guard/guard-test/compare/v0.6.0...v0.7.0)

### New feature

* [#35][] Support `include:` option to extend the load path of the test runner. ([@amiel][])

## 0.6.0 - November 3, 2012

[Full Changelog](https://github.com/guard/guard-test/compare/v0.5.0...v0.6.0)

### New feature

* [#34][] Support for `*_tests.rb`. ([@pastorius][])

## 0.5.0 - June 2, 2012

[Full Changelog](https://github.com/guard/guard-test/compare/v0.4.3...v0.5.0)

### Bug fix

* [#24][] Add note for Rails projects using profile/benchmark tests in README. ([@coderjoe][])

### Changes

* Updat for Guard 1.1. ([@rymai][])

### New feature

* [#20][] Add the `:rubygems` options for projects that don't use Bundler. ([@rymai][])

## 0.4.3 - December 19, 2011

[Full Changelog](https://github.com/guard/guard-test/compare/v0.4.2...v0.4.3)

### Bug fix

* [#21][] `Guard::Test::Notifier.notify` did not use :failed image if test results included errors but NO failures. ([@carlost][])

## 0.4.2 - November 19, 2011

[Full Changelog](https://github.com/guard/guard-test/compare/v0.4.1...v0.4.2)

### Bug fix

* [#19][] Fix "superclass mismatch for class Test (TypeError)" thanks to [@gertas][]. ([@rymai][])

## 0.4.1 - November 3, 2011

[Full Changelog](https://github.com/guard/guard-test/compare/v0.4.0...v0.4.1)

### Bugs fixes

* [#18][] Fix a conflict with test_benchmark that was preventing guard-test from running. ([@rymai][])
* [#11][] Fix a "No such file to load -- guard/notifier" when running guard without bundler. ([@rymai][])

## 0.4.0 - September 29, 2011

[Full Changelog](https://github.com/guard/guard-test/compare/v0.3.1...v0.4.0)

### Regression

* Remove support of [turn](https://github.com/guard/guard-spork) gem since "Turn is no longer compatible with TestUnit 2.0+. TestUnit and MiniTest are deverging and after some consideration it was decided that Turn's goal is to support Ruby's native test framework, whatever it may be." quoted from Turn's [release.txt](https://github.com/TwP/turn/blob/master/Release.txt). ([@rymai][])

### New feature

* New `:drb` option enabling the use of [`spork-testunit`](https://github.com/timcharper/spork-testunit) gem (be sure to use [guard-spork](https://github.com/guard/guard-spork) as well). ([@rymai][])

## 0.3.1 - September 11, 2011

[Full Changelog](https://github.com/guard/guard-test/compare/v0.3.0...v0.3.1)

### New feature

* [#13][] New `test_paths` option to look for test files under other paths than `test`. ([@Ask11][])

### Improvement

* [#15][] Simplify some checks. ([@dasch][])

## 0.3.0 - June 14, 2011

[Full Changelog](https://github.com/guard/guard-test/compare/v0.3.0.rc5...v0.3.0)

### Improvement

* Internal cleaning. ([@rymai][])

## 0.3.0.rc5 - June 9, 2011

[Full Changelog](https://github.com/guard/guard-test/compare/v0.3.0.rc4...v0.3.0.rc5)

### Bugs fixes

* Fix bug that was preventing tests from running. ([@rymai][])
* Fix the `fastfail` runner that was displaying a green dot even for a failing test. ([@rymai][])
* Remove the `:notification` option. Use the new Guard method instead. ([@rymai][])

### New feature

* Turn seems to work fine now... ([@rymai][])

### Improvement

* Consider `test_*.rb` as test files as well. ([@uk-ar][])

## 0.3.0.rc4 - June 3, 2011

[Full Changelog](https://github.com/guard/guard-test/compare/v0.3.0.rc3...v0.3.0.rc4)

### Bugs fix

* Add a require that was making the guard be fired by Guard! :'( ([@rymai][])

## 0.3.0.rc3 - June 3, 2011

[Full Changelog](https://github.com/guard/guard-test/compare/v0.3.0.rc2...v0.3.0.rc3)

### Bugs fix

* Actually make the tests run. ([@rymai][])

### Regression

* Turn doesn't want to run, so remove sentences that say that it is supported for now. Note: The code is still here, only the command line doesn't seem to output anything... ([@rymai][])

## 0.3.0.rc2 - June 2, 2011

[Full Changelog](https://github.com/guard/guard-test/compare/v0.1.6...v0.3.0.rc2)

### New features

* New `:cli` option (nil by default) to pass arbitrary CLI arguments to the Ruby/Turn command that runs the tests. ([@rymai][])
* New `:notification` option (true by default) to disable notification (Growl/Inotify). ([@rymai][])
* New `:all_on_start` option (true by default) to not run all the tests at startup. ([@rymai][])
* New `:all_after_pass` option (true by default) to run all tests after changed tests pass. ([@rymai][])
* New `:keep_failed` option (true by default) to keep failed tests until them pass. ([@rymai][])

### Improvements

* Add compatibility with 1.8.6, 1.8.7, 1.9.2, REE, Rubinius and JRuby. ([@rymai][])
* Internal changes inspired by [guard-minitest](https://github.com/guard/guard-minitest). ([@rymai][])

## 0.1.6 - January 24, 2011

[Full Changelog](https://github.com/guard/guard-test/compare/v0.1.5...v0.1.6)

### Bugs fix

* [#2][] Fixed a bug introduced in 0.1.5 where test/ was not added to the $LOAD_PATH. ([@rymai][])

## 0.1.5 - January 21, 2011

[Full Changelog](https://github.com/guard/guard-test/compare/v0.1.4...v0.1.5)

* Update gem dependencies. ([@rymai][])

## 0.1.4 - December 15, 2010

### Bugs fix

* [#1][] Include errors count to determine the "flag" to display in notification. ([@gregorymostizky][])

<!--- The following link definition list is generated by PimpMyChangelog --->
[#1]: https://github.com/guard/guard/issues/1
[#2]: https://github.com/guard/guard/issues/2
[#11]: https://github.com/guard/guard/issues/11
[#13]: https://github.com/guard/guard/issues/13
[#15]: https://github.com/guard/guard/issues/15
[#18]: https://github.com/guard/guard/issues/18
[#19]: https://github.com/guard/guard/issues/19
[#20]: https://github.com/guard/guard/issues/20
[#21]: https://github.com/guard/guard/issues/21
[#24]: https://github.com/guard/guard/issues/24
[#34]: https://github.com/guard/guard/issues/34
[#35]: https://github.com/guard/guard/issues/35
[#38]: https://github.com/guard/guard/issues/38
[#40]: https://github.com/guard/guard/issues/40
[#41]: https://github.com/guard/guard/issues/41
[@Ask11]: https://github.com/Ask11
[@amiel]: https://github.com/amiel
[@carlost]: https://github.com/carlost
[@coderjoe]: https://github.com/coderjoe
[@dasch]: https://github.com/dasch
[@djmaze]: https://github.com/djmaze
[@gertas]: https://github.com/gertas
[@gregorymostizky]: https://github.com/gregorymostizky
[@jgrau]: https://github.com/jgrau
[@pastorius]: https://github.com/pastorius
[@pgaertig]: https://github.com/pgaertig
[@rymai]: https://github.com/rymai
[@uk-ar]: https://github.com/uk-ar