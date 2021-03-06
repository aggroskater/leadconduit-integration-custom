# Change Log
All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

## [2.14.3] - 2017-06-06
### Fixed
- fix to parse reason text from JSON array response

## [2.14.2] - 2017-05-11
### Fixed
- compact arrays for SOAP transactions

## [2.14.1] - 2017-03-06
### Fixed
- fix to cookie header search to ignore case

## [2.14.0] - 2017-03-06
### Added
- add ability to capture cookie headers via `cookie_search_term`

## [2.10.0] - 2016-10-05
### Added
- added ability to override response `Content-Type` (issue #32)

## [2.9.1] - 2016-09-21
### Fixed
- support "capture" fields in HTML responses, too
- clean up "reason" text extracted from XML CDATA

## [2.9.0] - 2016-09-14
### Added
- Can now specify "capture" fields and mapped regular expressions with capture groups to populate them

## [2.8.4] - 2016-08-29
### Fixed
- `form_field.*` field names with brackets are correctly preserved (issue #8)

## [2.8.3] - 2016-08-25
### Fixed
- When all `json_property` values have a leading digit, assume the user wants a root array.

## [2.8.2] - 2016-07-09
### Fixed
- add `send_ascii` to SOAP integrations request variables

## [2.8.1] - 2016-07-09
### Fixed
- make `unidecode` a regular dependency (not devDependency)

## [2.8.0] - 2016-07-08
### Added
- support for request variable `send_ascii`: map "true" to this and all lead data will be transliterated to ASCII (e.g., ö -> o)

## [2.7.2] - 2016-06-09
### Fixed
- responses are now always treated as success if no outcome on match and no search term are specified

### Added
- addition of `json_parameter` and `extra_parameter` to JSON integration: "To 'stuff' the JSON into a parameter and send as Form URL encoded" (similar to XML integration's `xml_parameter`)

## [2.7.0] - 2016-05-24
### Added
- new request variable on `xml`: map additional parameters to `extra_parameter.*` when `xml_parameter` is set
- this changelog

## [0.1.0] - 2016-02-10
### Added
- Initial commit
