# TTY::Screen [![Gitter](https://badges.gitter.im/Join%20Chat.svg)][gitter]
[![Gem Version](https://badge.fury.io/rb/tty-screen.svg)][gem]
[![Build Status](https://secure.travis-ci.org/piotrmurach/tty-screen.svg?branch=master)][travis]
[![Code Climate](https://codeclimate.com/github/piotrmurach/tty-screen/badges/gpa.svg)][codeclimate]
[![Coverage Status](https://coveralls.io/repos/piotrmurach/tty-screen/badge.svg)][coverage]
[![Inline docs](http://inch-ci.org/github/piotrmurach/tty-screen.svg?branch=master)][inchpages]

[gitter]: https://gitter.im/piotrmurach/tty
[gem]: http://badge.fury.io/rb/tty-screen
[travis]: http://travis-ci.org/piotrmurach/tty-screen
[codeclimate]: https://codeclimate.com/github/piotrmurach/tty-screen
[coverage]: https://coveralls.io/r/piotrmurach/tty-screen
[inchpages]: http://inch-ci.org/github/piotrmurach/tty-screen

> Terminal screen size detection which works on Linux, OS X and Windows/Cygwin platforms and supports MRI, JRuby and Rubinius interpreters.

**TTY::Screen** provides independent screen size detection component for [TTY](https://github.com/piotrmurach/tty) toolkit.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'tty-screen'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install tty-screen

## 1. Usage

**TTY::Screen** allows you to detect terminal screen size by calling `size` method which returns [height, width] tuple.

```ruby
screen = TTY::Screen.new

screen.size     # => [51, 280]
screen.width    # => 280
screen.height   # => 51
```

You can also use above methods as class instance methods:

```ruby
TTY::Screen.size     # => [51, 280]
TTY::Screen.width    # => 280
TTY::Screen.height   # => 51
```

## Contributing

1. Fork it ( https://github.com/piotrmurach/tty-screen/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request

## Copyright

Copyright (c) 2014-2016 Piotr Murach. See LICENSE for further details.
