source 'https://rubygems.org'
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby '2.6.2'

gem 'bootsnap', '>= 1.4.2', require: false
gem 'jbuilder', '~> 2.7'
gem 'nokogiri', '>= 1.10.4'
gem 'pg', '>= 0.18', '< 2.0'
gem 'puma', '~> 3.12'
gem 'rails', '~> 6.0.0'
gem 'sass-rails', '~> 5'
gem 'stackprof'
gem 'tailwindcss'
gem 'turbolinks', '~> 5'
gem 'webpacker', '~> 4.0'

group :development, :test do
  gem 'byebug', platforms: %i[mri mingw x64_mingw]
  gem 'factory_bot_rails'
  gem 'ffaker'
  gem 'simplecov', require: false
end

group :development do
  gem 'annotate'
  gem 'flamegraph'
  gem 'listen', '>= 3.0.5', '< 3.2'
  gem 'rack-mini-profiler', require: false
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
  gem 'web-console', '>= 3.3.0'
end

group :test do
  gem 'capybara', '>= 2.15'
  gem 'selenium-webdriver'
  gem 'webdrivers'
end
