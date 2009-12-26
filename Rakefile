require 'rubygems'
require 'hoe'

Hoe.spec 'oauth' do |p|
  developer 'Pelle Braendgaard', "oauth-ruby@googlegroups.com"
  developer 'Blaine Cook', nil
  developer 'Larry Halff', nil
  developer 'Jesse Clark', nil
  developer 'Jon Crosby', nil
  developer 'Seth Fitzsimmons', nil

  self.readme_file      = 'README.rdoc'
  self.extra_rdoc_files = Dir['*.rdoc']

  extra_deps      << ['ruby-hmac','>= 0.3.1']
  extra_deps      << ['typhoeus']

  %w{ actionpack rack mocha }.each do |lib|
    extra_dev_deps  << [lib]
  end
end

Dir['tasks/**/*.rake'].each { |t| load t }
