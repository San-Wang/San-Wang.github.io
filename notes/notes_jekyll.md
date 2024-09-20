# Jekyll Learning Note

## Glossary
* Ruby: open source programming language with a focus on simplicity and productivity. With following famous areas:
    * Web development: one of Ruby’s claims to fame because of the popular web development framework `Ruby on Rails`
    * Static site generation: Jekyll was the first static site generator and is still the most popular. Github’s founder, Tom Preston-Werner, created Jekyll and made it the default way to publish content on Github
    * Many others
* Jekyll: a popular static site generator, is written in Ruby
* gem: packages of Ruby code 
* bundler: a tool used for managing gem dependencies for Ruby projects

## Launch Website Locally

Prerequisites:
* install jekyll: https://jekyllrb.com/docs/installation/macos/
* install gems listed in Gemfile (can delete Gemfile.lock first): `bundle install`  

Launch site locally:
* `bundle exec jekyll serve`
* open `http://localhost:4000`


### Troubleshoot:

>I got error `bundler: command not found: jekyll` when running `bundle exec jekyll serve`:  
Solution: 
1. I updated Gemfile to `gem "jekyll", "~> 4.3.4"`, which I got from trying out creating new Jekyll site  
2. delete Gemfile.lock and then run `bundle install`

## References
* https://jekyllrb.com/docs/
* https://chaochungkuo.github.io/posts/jekyll-intro/
