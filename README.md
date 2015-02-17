## Sensu-Plugins-pushover

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-pushover.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-pushover)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-pushover.svg)](http://badge.fury.io/rb/sensu-plugins-pushover)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-pushover/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-pushover)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-pushover/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-pushover)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-pushover.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-pushover)

## Functionality

## Files
 * bin/handler-pushover

## Usage

```
{
  "pushover": {

    "_comment": "Single userkey / token pair",
    "userkey": "12345",
    "token": "54321",

    "_comment": "Multiple userkey / token pairs",
    "keys": [
      {
        "userkey": "abcdef",
        "token": "fedcab"
      },
      {
        "userkey": "ghijkl",
        "token": "lkjihg"
      }
    ]
  }
}
```
## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-pushover -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-pushover`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-pushover' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-pushover' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
