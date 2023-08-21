source 'https://rubygems.org'
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby '3.2.2'

# --------------------------- Application gems --------------------------- #
# Add application gems here!
gem 'concurrent-ruby'
gem 'dry-struct'
gem 'dry-types'
gem 'rails_event_store', '~> 2.9.1'
# --------------------------- Application gems --------------------------- #

# --------------------------- Base gems --------------------------- #
gem 'rails', '~> 7.0.6'
gem 'pg', '~> 1.4.5'
gem 'activerecord-postgis-adapter'
gem 'puma', '~> 5.0'
gem 'tzinfo-data', '~> 1.2022', '>= 1.2022.7'
gem 'bootsnap', require: false
gem 'scenic'

gem 'dalli'
gem 'kaminari'
gem 'oj'
gem 'http'
gem 'lograge'

group :development, :test do
  gem 'byebug', platforms: %i[ mri mingw x64_mingw ]
  gem 'factory_bot_rails'
  gem 'fuubar'
  gem 'rspec-rails', '~> 6.0.0'
  gem 'rubocop', require: false
  gem 'rubocop-rspec', require: false
end

group :development do
  gem 'listen', '~> 3.2'
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
end

group :test do
  gem 'database_cleaner-active_record'
  gem 'pry', '~> 0.14.2'
  gem 'rspec'
  gem 'simplecov', require: false
  gem 'webmock'
end
# --------------------------- Base gems --------------------------- #
