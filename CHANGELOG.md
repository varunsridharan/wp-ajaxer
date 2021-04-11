# 📝  Change Log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## 1.8.2 - 22/06/2019
### Added
* Option To Trigger Ajax For Non Logged in users if ajax is set to `single=>true`

## 1.8.1 - 20/06/2019
### Fixed
* Minor Bug

## 1.8 - 20/06/2019
### Changed
* Changed some methods from normal to final.
* `has_post` - method made public
* `has_get` - method made public
* `has_request` - method made public
* `validate_request` - method made public

## 1.7 - 19/06/2019
### Added
* `json_error($data,$status_code)` -> Triggers `wp_send_json_error`
* `json_success($data,$status_code)` -> Triggers `wp_send_json_success`
* `validate_post($key,$error)` -> Checks if given key is exits in **$_POST** if not send an error
* `validate_get($key,$error)` -> Checks if given key is exits in **$_GET** if not send an error

## 1.6 - 07/05/2019
### Added
* `class_exists` checks in php

## 1.5 - 07/05/2019
### Changed
* Updated

## 1.4 - 13/04/2019
### Fixed
* Added Single Ajax Request Option.

## 1.3 - 14/01/2019
### Fixed
* Issue With Autoloader Fixed.

## 1.2 - 20/12/2018
### Added
* Composer PSR4 Standards Autoloader Support

## 1.1 - 20/12/2018
### Added
* Composer Autoload Support

## 1.0 - 17/12/2018
### First Release


<!--
## Unreleased

## 1.0 - 01/02/2020
### Added

### Changed

### Deprecated

### Removed

### Fixed

### Security

-->
