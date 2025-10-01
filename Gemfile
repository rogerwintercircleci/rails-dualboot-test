# frozen_string_literal: true

# Helper method for dual boot
def next?
  File.basename(__FILE__) == "Gemfile.next"
end

source "https://rubygems.org"

# Rails version dual boot configuration
if next?
  gem 'rails', '~> 8.0.0'
else
  gem 'rails', '~> 7.2.2'
end

# Common gems
gem 'sqlite3', '~> 1.4'
gem 'puma', '>= 5.0'

# Testing gems
group :development, :test do
  gem 'rspec-rails'
end
