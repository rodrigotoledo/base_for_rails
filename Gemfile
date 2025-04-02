# frozen_string_literal: true

source "https://rubygems.org"

# Rails
gem "rails", github: "rails/rails", branch: "main"

# Database
gem "sqlite3", ">= 2.1"

# Web server
gem "puma", ">= 5.0.3"

# Asset management
gem "propshaft"
# gem "sprockets-rails", ">= 2.0.0", require: false  # May conflict with Rails 8

# Hotwire
gem "importmap-rails", ">= 1.2.3"
gem "stimulus-rails"
gem "tailwindcss-rails"
gem "turbo-rails"
# gem "dartsass-rails"

# Caching and Queuing
gem "solid_cable"
gem "solid_cache"
gem "solid_queue"

# Authentication and Security
gem "authentication-zero"
gem "bcrypt", "~> 3.1.11", require: false
gem "email_validator"
gem "jwt", "~> 2.5"

# Utilities
gem "launchy"
gem "prism"
gem "redis", ">= 4.0.1", require: false
gem "redis-namespace"
gem "useragent", require: false

# Performance
gem "rack-cache", "~> 1.2"
gem "rack-cors"

# Rails enhancements
gem "kamal", require: false
gem "thruster", require: false

# Windows platform gems
gem "tzinfo-data", platforms: %i[mingw mswin x64_mingw jruby]
gem "wdm", ">= 0.1.0", platforms: [:windows]

# Essential Gems
gem "bootsnap", ">= 1.4.4", require: false
# gem "webrick", require: false
# gem "jbuilder", require: false

# HTTP and WebSocket Clients
gem "aws-sdk-sns", require: false

# Icon Libraries
gem "rails_heroicon"

# Platform-specific Gems
gem "connection_pool", require: false
gem "libxml-ruby", platforms: :ruby
gem "msgpack", ">= 1.7.0", require: false
gem "rexml", require: false

# Version control of rack
rack_version = ENV.fetch("RACK", "~> 3.0")
if rack_version == "head"
  gem "rack", git: "https://github.com/rack/rack.git", branch: "main"
else
  gem "rack", rack_version
end

gem "rubocop-rails-omakase", require: false

# Development and Test
group :development, :test do
  gem "httpclient", github: "nahi/httpclient", branch: "master", require: false
  gem "webmock"
  gem "websocket-client-simple", github: "matthewd/websocket-client-simple", branch: "close-race", require: false

  gem "debug", platforms: %i[mri windows], require: "debug/prelude"
  gem "dotenv"
  gem "dotenv-rails"
  gem "pry"

  # Static analysis for security vulnerabilities
  gem "brakeman", require: false

  # Development tools
  gem "annotate"
  gem "bundler-audit"
  gem "factory_bot_rails"
  gem "faker"
  gem "foreman"
  gem "letter_opener"
  gem "letter_opener_web"
  gem "rufo"

  gem "guard-rspec", require: false
  gem "rspec-rails"

  gem "sidekiq", require: false
  gem "sidekiq-cron"
end

# Development only
group :development do
  gem "hotwire-spark"
  gem "web-console"
  # gem "rack-mini-profiler"  # May conflict with Rails 8
  # gem "spring"              # May conflict with Rails 8
end

# Test only
group :test do
  gem "database_cleaner-active_record"
  gem "rspec-json_expectations"
  gem "shoulda-matchers"
  gem "simplecov", require: false
end

# Linting
group :lint do
  gem "syntax_tree", "6.1.1", require: false
end

# Documentation
group :doc do
  gem "rouge"
  gem "rubyzip", "~> 2.0"
end

# Storage
group :storage do
  gem "aws-sdk-s3", require: false
  gem "azure-storage-blob", "~> 2.0", require: false
  gem "google-cloud-storage", "~> 1.11", require: false
  gem "image_processing", "~> 1.2"
end
