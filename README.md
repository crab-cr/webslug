# webslug

inspired by "slug" from npm, but optimized for my slugs use case. Requests for more slug examples are welcome!
```
require "webslug"

Iom::WebSlug.slug("i ♥ unicode").should eq "i-love-unicode"
Iom::WebSlug.slug("I ♥ UNICODE").should eq "i-love-unicode"
Iom::WebSlug.slug("i <3 unicode").should eq "i-love-unicode"
Iom::WebSlug.slug("компютъра").should eq "kompyutura"
Iom::WebSlug.slug("unicode ♥ is ☢").should eq "unicode-love-is-radioactive"
Iom::WebSlug.slug("http://www.example.com").should eq "www-example-com"
Iom::WebSlug.slug("Schlotsky's").should eq "schlotskys"
```
## Installation

1. Add the dependency to your `shard.yml`:

   ```yaml
   dependencies:
     webslug:
       github: iomcr/webslug
   ```

2. Run `shards install`

## Usage

```crystal
require "webslug"
```

TODO: Write usage instructions here

## Development

TODO: Write development instructions here

## Contributing

1. Fork it (<https://github.com/iomcr/webslug/fork>)
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request

## Contributors

- [Iomcr](https://github.com/iomcr) - creator and maintainer
