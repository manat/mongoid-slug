source 'https://rubygems.org'

gemspec name: 'mongoid-slug'

case version = ENV['MONGOID_VERSION'] || '5.0.1'
when 'HEAD'
  gem 'mongoid', github: 'mongodb/mongoid'
  gem 'mongoid_paranoia'
  gem 'mongoid-observers'
when '5.0.0'
  gem 'mongoid', '5.0.0'
  gem 'mongoid_paranoia'
  gem 'mongoid-observers'
when /^5/
  gem 'mongoid', '~> 5.0'
  gem 'mongoid_paranoia'
  gem 'mongoid-observers'
when /^4/
  gem 'mongoid', '~> 4.0'
  gem 'mongoid_paranoia'
  gem 'mongoid-observers'
when /^3/
  gem 'mongoid', '~> 3.1'
else
  gem 'mongoid', version
end
