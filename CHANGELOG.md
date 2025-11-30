# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- Added install_docker role. 
- Added deploy_db playbook. 
- Added deploy_app playbook. 

### Changed
- Changed nessecary vairables.
- Split appserver instances to appserver1 and appserver2.
- Edited load-balancer.conf to dynamically fetch all appservers.
- Switched from a Debian VM to a Ubuntu VM.
- SSH keys are not taken from GitHub accounts.

## [11.0.0]

### Added

- This CHANGELOG file.
- Dockerfile_prod. To run the microblog via docker. 
- boot.sh. 
- Dockerfile_test. To run the tests via docker.
- Docker compose file to run the microblog, MySQL and tests
- boot_test.sh.
- CI pipeline setup for Github Actions
- Actions badge in README
- CD pipeline setup for Github Actions
- Followers functionality for the webpage.
