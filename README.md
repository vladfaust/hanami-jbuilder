# hanami-jbuilder

Adds support for rendering Jbuilder templates using Tilt, fixed for Hanami

## Installation

Add this line to your application's Gemfile:

    gem 'tilt-jbuilder', github: 'vladfaust/hanami-jbuilder'

And then execute:

    $ bundle

## Usage

1. `require 'tilt/jbuilder'` somewhere
2. Remove rendering layout or it will override your *.json.jbuilder files!
```ruby
module Api
  class Application < Hanami::Application
    configure do
      # The layout to be used by all views
      # layout :application # COMMENT IT
```
3. Just add *.json.jbuilder files in templates directory and it'll work

## Contributing
1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## Credits

[![Sticksnleaves](https://s3.amazonaws.com/sticksnleaves-assets/snl-logo-116x116.png)](http://www.sticksnleaves.com)

tilt-jbuilder is maintained and funded by [Sticksnleaves](http://www.sticksnleaves.com)
