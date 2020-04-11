# TwitterEmbed

Crawl Twitter's embed HTML with no limit.

## Installation

Add this line into the Gemfile:

```ruby
gem 'twitter_embed'
```

And then execute:

    $ bundle install

Or manually install it:

    $ gem install twitter_embed
    
Images need to be reloaded therefore it is necessary to add TwitterEmbed to application.js:

    //= require twitter_embed

And to retain twitter's design, add TwitterEmbed to application.css:

    *= require twitter_embed

## Usage

Retrieve tweet's HTML by providing the tweet's ID.
    
    > TwitterEmbed::Tweet.html_str("1240688751082221568")
Theme and language can also be specified. (defaults: language is 'en', theme is 'light')
    
    > TwitterEmbed::Tweet.html_str("1246619311638282242",lang: "ja", theme: "dark")
You can also check if the tweet exists by prodiving the link.
    
    > TwitterEmbed::Tweet.is_exists?("https://twitter.com/rails/status/1240688751082221568")
    
## Contributing

Bug reports are welcome on GitHub at https://github.com/wwwfernand/twitter_embed.
