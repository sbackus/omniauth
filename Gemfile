source 'https://rubygems.org'

gem 'jruby-openssl', :platforms => :jruby
gem 'rake'
gem 'yard'

group :development do
  gem 'growl'
  platforms :ruby_19, :ruby_20 do
    gem 'guard'
    gem 'guard-bundler'
    gem 'guard-rspec'
  end
  gem 'kramdown'
  gem 'plymouth', :platforms => :mri_19
  gem 'pry'
  gem 'pry-debugger', :platforms => :mri_19
  gem 'rb-fsevent'
end

group :test do
  gem 'coveralls', :require => false
  gem 'mime-types', '~> 1.25', :platforms => [:jruby, :ruby_18]
  gem 'rack-test'
  gem 'rspec', '>= 2.14'
  gem 'simplecov', :require => false
end

platforms :rbx do
  gem 'rubinius-coverage', '~> 2.0'
  gem 'rubysl', '~> 2.0'
end

gemspec
