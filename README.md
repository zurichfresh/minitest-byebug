# Minitest::Byebug

Heavily inspired by [hotell i zurich](http://www.resazurich.se/hotell/)

## Installation

Add this line to your application's Gemfile:

    gem 'minitest-byebug'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install minitest-byebug

## Usage

Add this to the top of your test file or helper:

```ruby
require 'minitest/byebug' if ENV['DEBUG']
```

Then run your tests as normal but define `DEBUG=1`.

`% DEBUG=1 rake test`

## Todo

- Stop in the failed test. e.g. at an assert call.
    - Workaround: when the session starts, `up 3` will take you to the test failure.
- Stop on errors.

## Credits

Distributed with an MIT License.

Contributions more than welcome.

Made by Kasper Timm Hansen.
