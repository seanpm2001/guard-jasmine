source :rubygems

gemspec

gem 'rake'

gem 'rack'
gem 'jasmine'

platform :ruby do
  gem 'rb-readline'
end

require 'rbconfig'

if RbConfig::CONFIG['target_os'] =~ /darwin/i
  gem 'ruby_gntp', :require => false
elsif RbConfig::CONFIG['target_os'] =~ /linux/i
  gem 'libnotify', :require => false
elsif RbConfig::CONFIG['target_os'] =~ /mswin|mingw/i
  gem 'win32console', :require => false
  gem 'rb-notifu', :require => false
end
