# Changelog
## 3.4.2 -- 2025-08-28
### Changed
* Invalid values in disabled fields are now ignored. ([#609](https://github.com/fwdekker/intellij-randomness/pull/609))

### Fixed
* Reproduced and (hopefully) fully fixed "Must be not computed before that call" exception. Thanks to the many anonymous issue reporters! ([#R44](https://github.com/fwdekkerbot/intellij-randomness-issues/issues/44))
* Limited UUID date-times to be between 1970-01-01 and 5236-03-31 because date-times outside of this range were not generated correctly due to limitations in the underlying UUID generator library. Thanks to [Czajka667](https://github.com/Czajka667) for reporting the issue. ([#606](https://github.com/fwdekker/intellij-randomness/pull/606)) ([#609](https://github.com/fwdekker/intellij-randomness/pull/609))
* Fixed settings not jumping to invalid field if that field is part of a decorator (i.e. array, fixed length, or surround with). ([#610](https://github.com/fwdekker/intellij-randomness/pull/610))
