require "bundler/setup"
require "rspec/core/rake_task"
require "rdoc/task"

Bundler::GemHelper.install_tasks

RSpec::Core::RakeTask.new do |t|
  t.rspec_opts = "--color --format progress"
end

RDoc::Task.new do |t|
  t.rdoc_dir = "rdoc"
  t.title    = "DelegatesAttributesTo"
  t.options += ["--line-numbers", "--inline-source"]
  t.rdoc_files.include("README", "lib/**/*.rb")
end

task :default => :spec
