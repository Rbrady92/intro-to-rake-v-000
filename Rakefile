task :environment do 
  require_relative './config/environment'
end 

desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

namespace :db do
  desc 'migrate changes to your database'
  rask :migrate => :environment do 
    Student.create_table
  end 

  desc 'seed the db with dummy data'
  task :seed do 
    require_relative './db/seedsrb'
  end 
end


