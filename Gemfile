source 'https://rubygems.org'

gem "jekyll", "~> 4.3.3"
gem "just-the-docs", "~> 0.7.0"

group :jekyll_plugins do
  gem "jekyll-default-layout"
  gem "jekyll-seo-tag"
  gem "jekyll-feed"
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]
