source 'https://rubygems.org'

require 'json'
require 'open-uri'
versions = JSON.parse(open('https://pages.github.com/versions.json').read)

gem 'github-pages', versions['github-pages']
gem 'rake'

gem 'pygments.rb'

# gem 'jemoji'
gem "jekyll"
# gem "jekyll-github-metadata"
gem "jekyll-octicons"

# gem 'jekyll-latex'
# version conflict
gem "addressable", ">= 2.8.0"
gem "nokogiri", ">= 1.12.5"
