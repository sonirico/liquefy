# liquefy

`liquefy` is a [liquid][1] filter for parsing and rendering input text that
might implement unprocessed liquid tags within Ruby applications. It has been
made with [Jekyll][3] in mind mainly.

## Rubygem

You can clone this repo and use `gem build liquefy.gemspec && gem install
liquefy-*.*.*.gem` in order to install it locally. Anyway, a [remote][2] gem
is also provided.

## Jekyll

If your need involve a Jekyll site just add the gem to your `jekyll-plugins`
group, like:

```ruby
group :jekyll_plugins do
    gem "liquefy", "~> 0.1.2"
end
```

Finally don't forget to run `bundle install|update`. Use `gem` for not 
"bundled" apps

## Usage

```liquid
    {{ text_with_liquid_tags | liquefy }}
```

[1]: https://shopify.github.io/liquid/
[2]: https://rubygems.org/gems/liquefy
[3]: http://jekyllrb.com/
