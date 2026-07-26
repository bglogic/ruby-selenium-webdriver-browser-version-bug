# README

This is reproducible code to demonstrate a `selenium-webdriver` bug in Linux where it doesn't read the specified `browser_version` driver option. It is a basic Rails project `rails new selenium_browser_version` with a single view and a single system test.

The "dev" channel is specified for the `browser_version` in the chrome driver options at `test/application_system_test_case.rb`.

Have a "stable" Google Chrome installed in your system then clone this repo and run `bin/rails test:all`. Selenium will ignore the specified chrome driver options and download a ChromeDriver matching your locally installed Chrome to run the tests.
