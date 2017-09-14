source 'http://rubygems.org'

gemspec

rails_version = ENV["RAILS_VERSION"] || "default"

rails = case rails_version
when "master"
  { github: "rails/rails" }
when "default"
  "~> 4.2"
else
  "~> #{rails_version}"
end

if RUBY_VERSION < "2.0"
  gem 'mime-types', '<= 2.99.1'
end

gem 'actionmailer', rails
gem 'activesupport', rails

# Add dependencies to develop your gem here.
# Include everything needed to run rake, tests, features, etc.
group :development do
  gem 'rake'
end
