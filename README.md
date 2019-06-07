### Pre-Requirements

- Fork this github repository into your account (You will find a "fork" icon on the top right corner)
- Clone the forked repository that exists in **your github account** into your local machine

### Requirements

- Ruby 2.4+ (It is already installed if you are using Mac OS X). If you need to install ruby follow the instructions on [rvm.io](https://rvm.io/rvm/install)

### Setup the environment

Install bundler 1.17.2 if you don't have it already installed

`sudo gem install bundler -v 1.17.2`

Verify that you have the right version by running `bundler --version`

If you have more recent versions of bundler, unistall them with `gem uninstall bundler` until the most up to date and default version of bundler is 1.17.2

### Install dependencies

- Execute `bundle install`

### Run the tests

- Execute `rspec`

### Provider Step 0 (Setup)

Get familiraised with the code

![System diagram](https://github.com/doktor500/pact-workshop-provider/blob/master/resources/system-diagram.png "System diagram")

There are two microservices in this system. A `consumer` and a `provider` (this repository).

The "provider" is a PaymentService that validates if a credit card number is valid in the context of that system.

The "consumer" only makes requests to PaymentService to verify payment methods.

Navigate to the [Consumer](https://github.com/doktor500/pact-workshop-consumer/) repository and follow the instructions in the **Consumer's** readme file
