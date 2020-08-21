# Drupal 9 Testing Environment
It runs Drupal's PHPUnit test suites on DDEV

## Install dependencies
* `composer install`
* `ddev start`

## Running tests

### Run all tests for a module
* `ddev ssh`
* `../vendor/bin/phpunit -c core core/modules/action`

### Run Functional tests
* `ddev ssh`
* `../vendor/bin/phpunit -c core core/modules/big_pipe/tests/src/FunctionalJavascript`

### Run tests on custom modules
* `ddev ssh`
* `../vendor/bin/phpunit -c core web/modules/custom/my_module`
