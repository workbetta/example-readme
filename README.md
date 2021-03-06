# MailFace Ruby SDK

[![Gem Version](http://img.shields.io/gem/v/twilio-ruby.svg)][gem]
[![Build Status](http://img.shields.io/travis/twilio/twilio-ruby.svg)][travis]
[![Contact Support](https://img.shields.io/badge/contact-support-blue.svg)][support]

MailFace is an API for mailing your face to any email address. With one simple API call you can send your face  and get first class delivery. 

For more details see the [Ruby documentation](https://mailface.xyz/docs/ruby) on [MailFace.xyz](https://mailface.xyz).

## Installation

This gem requires Ruby 2.1+. You can install install it directly or via bundler.

```ruby
gem install 'mailface'
```

__Next__: [Get Started with the Ruby SDK.](https://mailface.xyz/docs/ruby/get_started/initialize) 

## Getting Started

To send your first face via email you will need to [register for MailFace](https://mailface.xyz/register) and [set up your first application](https://dashboard.mailface.xyz/applications).

```ruby
mailface = MailFace.new({
  app_id: '[YOUR_APP_ID]',
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
mailface = MailFace.new(app_id: '...', api_key: '...', api_secret: '...')

# Alternative: Initialize using environment variables
# * MAILFACE_API_KEY
# * MAILFACE_API_SECRET
mailface = MailFace.new
```

Your credentials can be found on the [MailFace dashboard](https://dashboard.mailface.xyz/api_keys). [Sign up](https://mailface.xyz/register) for an account today. 

__Next__: [Learn more about our initializing the Ruby SDK](https://mailface.xyz/docs/ruby/get_started_initialize) in our documentation.

## Documentation

MailFace is a powerful tool and our documentation is here to get you started today.

* [Get Started](https://mailface.xyz/docs/ruby/get_started) documentation
  * [Initialize the SDK](https://mailface.xyz/docs/ruby/get_started/initialize)
  * [Send a face](https://mailface.xyz/docs/ruby/get_started/send_face)
  * [Send to multiple faces](https://mailface.xyz/docs/ruby/get_started/send_multiple_faces)
  * [Check the status of a face mailed](https://mailface.xyz/docs/ruby/get_started/check_status)

Alternatively, head over to our [Reference](https://mailface.xyz/docs/ruby/reference) documentaton for in-depth information about every SDK method, it's arguments and return types.

## Contributing

Want to contribute to this library? Read our [contributor guidelines](CONTRIBUTING.md) to get set up.

## License

This library is released under the [MIT License](LICENSE).

## Help

Our [developer support team](https://mailface.xyz/developers) is here to help you. You can find us on [Twitter](https://twitter.com/mailfacexyz), [StackOverflow](#), and [email](#).

[gem]: https://rubygems.org/gems/twilio-ruby
[travis]: http://travis-ci.org/twilio/twilio-ruby
[support]: http://mailface.xyz/support
