# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]
- Added node-exporter setup
- Added prometheus setup
- Added grafana setup
- Added prometheus flask
- Added alertmanager to prometheus
- Changed the ip adresses in prometheus to match the VM:s
- Added reverse proxy to nginx to point to Grafana
- Added granfana config to make reverse proxy work
- Changed ports to match security

## [13.0.11]

### Added
- Added Bandit to requirement list. 
- Added "make bandit" command to run bandit on app/. 
- Added "make trivy" command to run trivy on image and fs. 
- Added security-check.yml workflow to run before the CD workflow. 
- Changed port access on VM:s
- Updated requirements to not have security issues
- Ignored errors from dockle and trivy

## [12.0.16]

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
- Updated CD workflow to deploy application. 

## [11.0.1]

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

[Unreleased]: https://github.com/Nalanys/DV1673_microblog/tree/dev
[13.0.11]: https://github.com/Nalanys/DV1673_microblog/tree/13.0.11
[12.0.16]: https://github.com/Nalanys/DV1673_microblog/tree/12.0.16
[11.0.1]: https://github.com/Nalanys/DV1673_microblog/tree/11.0.1
