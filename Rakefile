$LOAD_PATH.unshift("lib")

require "challenge"
require "rspec/core/rake_task"

RSpec::Core::RakeTask.new(:spec)

task :example do
  Harness.run(SomeonesAttempt.new, numbers_to_test: 1..3)
end

task default: :example

# Add your own rake task below:

task :tuzz do
  Harness.run(Tuzz.new)
end
