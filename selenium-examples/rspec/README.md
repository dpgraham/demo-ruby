# Ruby-RSpec-Selenium
[![Travis Status](https://travis-ci.org/saucelabs-sample-test-frameworks/Ruby-RSpec-Selenium.svg?branch=master)](https://travis-ci.org/saucelabs-sample-test-frameworks/Ruby-RSpec-Selenium)

This code is provided on an "AS-IS” basis without warranty of any kind, either express or implied, including without limitation any implied warranties of condition, uninterrupted use, merchantability, fitness for a particular purpose, or non-infringement. Your tests and testing environments may require you to modify this framework. Issues regarding this framework should be submitted through GitHub. For questions regarding Sauce Labs integration, please see the Sauce Labs documentation at https://wiki.saucelabs.com/. This framework is not maintained by Sauce Labs Support.

## Environment Setup

1. Global Dependencies
    * [Install Ruby](http://watir.com/guides/ruby/)
    * [Install Git](https://github.com/saucelabs-training/Getting-Started-with-Selenium/blob/master/README.md#install-git)
    * Clone This Repo
    ```
    $ git clone https://github.com/saucelabs-training/demo-ruby.git
    ```
    * Install bundler
    ```
    $ gem install bundler
    ```

2. Sauce Credentials
    * Add the following Sauce Labs Credentials as environmental variables
    (specific details will vary depending on Operating System).
    ```
    $ export SAUCE_USERNAME=<your Sauce Labs username>
    $ export SAUCE_ACCESS_KEY=<your Sauce Labs access key>
    ```

3. Navigate to the `rspec` directory (`/selenium-examples/rspec/`)
	```
	$ cd selenium-examples/rspec
	```
4. Install the `gem` packages
	```
	$ bundle install
	```

## Running Tests

* Run tests in parallel on default configuration:
	```
	$ bundle exec rake
	```
* Run in parallel on a specified configuration (see `/spec/Rakefile` for the available tasks)
	```
	$ bundle exec rake windows_10_edge
	```
* Sauce Labs Demo execution:
	```
	$ bundle exec rake sauce_demo
	```

## Watch Your Tests Run

[Sauce Labs Dashboard](https://app.saucelabs.com/dashboard)
