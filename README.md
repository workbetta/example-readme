# MailFace Ruby SDK

[![Gem Version](http://img.shields.io/gem/v/twilio-ruby.svg)][gem]
[![Build Status](http://img.shields.io/travis/twilio/twilio-ruby.svg)][travis]

MailFace is an API for mailing your face to your customers. With one simple API call you can send your face to any email address and get first class delivery. 

For more details see the [Ruby documentation](https://mailface.xyz/docs) on [MailFace.xyz](https://mailface.xyz).

## Installation

This gem requires Ruby 2.1+. You can install install it directly or via bundler.

```ruby
gem install 'mailface'
```

__Next__: [Get Started with the Ruby SDK.](https://mailface.xyz/docs/ruby/get_started/initialize) 

## Getting Started

To send your first face via email:

```ruby
mailface = MailFace.new({
  api_key: '[YOUR_API_KEY]',
  api_secret: '[YOUR_API_SECRET]'
})

mailface.send({
  email: 'recipient@example.com',
  face: 'path/to/yourface.png'
}) 
```

__Next__: [Learn more about our sending faces](https://mailface.xyz/docs/ruby/get_started/send_face) with our Ruby SDK.

## Initialization

The client follows the [12-factor](http://12factor.net/config) apps principle and can be either set directly or via environment variables.

```ruby
# Initialize using parameters
mailface = MailFace.new(api_key: '...', api_secret: '...')

# Alternative: Initialize using environment variables
# * MAILFACE_API_KEY
# * MAILFACE_API_SECRET
mailface = MailFace.new
```

__Next__: [Learn more about our initializing the Ruby SDK](https://mailface.xyz/docs/ruby/get_started_initialize) in our documentation.

## Documentation





[gem]: https://rubygems.org/gems/twilio-ruby
[travis]: http://travis-ci.org/twilio/twilio-ruby
