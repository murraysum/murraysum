# Rakefile
require "rake"

namespace :assets do

  desc "Compile static site"
  task :precompile do
    Rake::Task["assets:clean"].invoke
    sh "bundle exec nanoc compile"
  end

  desc "Remove compiled site"
  task :clean do
    sh "rm -rf #{File.dirname(__FILE__)}/output/*"
  end

end