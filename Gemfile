source ENV['GEM_SOURCE'] || "https://rubygems.org"

group :unit_tests do
  gem 'rake',                                              :require => false
  gem 'rspec', '~> 3.1.0',                                 :require => false
  gem 'rspec-puppet',                                      :require => false
  gem 'puppetlabs_spec_helper',                            :require => false
  gem 'puppet-lint', '1.0.1',                              :require => false
end

group :development do
  gem 'guard-rake',  :require => false
end

if facterversion = ENV['FACTER_GEM_VERSION']
  gem 'facter', facterversion, :require => false
else
  gem 'facter', :require => false
end

if puppetversion = ENV['PUPPET_GEM_VERSION']
  gem 'puppet', puppetversion, :require => false
else
  gem 'puppet', :require => false
end
