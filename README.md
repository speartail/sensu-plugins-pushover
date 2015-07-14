## Sensu-Plugins-pushover

[ ![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-pushover.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-pushover)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-pushover.svg)](http://badge.fury.io/rb/sensu-plugins-pushover)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-pushover/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-pushover)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-pushover/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-pushover)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-pushover.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-pushover)
[ ![Codeship Status for sensu-plugins/sensu-plugins-pushover](https://codeship.com/projects/79576aa0-edb0-0132-5c33-1efd3f886df2/status?branch=master)](https://codeship.com/projects/84061)

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

[Installation and Setup](https://github.com/sensu-plugins/documentation/blob/master/user_docs/installation_instructions.md)

## Notes
