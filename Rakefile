task :default => :spec

desc 'Run specs (with story style output)'
task 'spec' do
  sh 'bacon -s spec/*_spec.rb'
end

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gemspec|
    gemspec.name = "heroku-nav"
    gemspec.summary = ""
    gemspec.description = ""
    gemspec.homepage = "http://heroku.com"
    gemspec.authors = ["David Dollar", "Pedro Belo", "Raul Murciano", "Todd Matthews"]
    gemspec.email = ["david@heroku.com", "pedro@heroku.com", "raul@heroku.com", "todd@heroku.com"]

    gemspec.add_development_dependency(%q<baconmocha>, [">= 0"])
    gemspec.add_development_dependency(%q<sinatra>, [">= 0"])
    gemspec.add_development_dependency(%q<rack-test>, [">= 0"])
    gemspec.add_dependency(%q<rest-client>, [">= 1.0"])
    gemspec.add_dependency(%q<json>, [">= 0"])

    gemspec.version = '0.1.24'
  end
rescue LoadError
  puts "Jeweler not available. Install it with: gem install jeweler"
end
