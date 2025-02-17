Pending Release Notes
=====================


Updates / New Features
----------------------

CI

* Updated CI unittests workflow to include codecov reporting.
  Reduced CodeCov report submission by skipping this step on scheduled runs.

* Update GitHub actions workflows with pinned python versions to use 3.7.

* Update code-cov action usage to use v3.

* Added properties file for use with SonarQube and SonarCloud.

Dependencies

* Updated minimum required python version to 3.7 to follow python end of life.

* Updated development abstract dep versions to "*" since we do not currently
  require any specific versions.

Documentation

* Updated CONTRIBUTING.md to reference smqtk-core's CONTRIBUTING.md file.

Fixes
-----

CI

* Modified CI unittests workflow to run for PRs targeting branches that match
  the `release*` glob.

Dependency Versions

* Updated the locked version of urllib3 to address a security vulnerability.

* Updated the developer dependency and locked version of ipython to address a
  security vulnerability.

* Removed `jedi = "^0.17.2"` requirement since recent `ipython = "^7.17.3"`
  update appropriately addresses the dependency.
