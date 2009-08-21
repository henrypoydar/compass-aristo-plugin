require 'rubygems'
require 'rake'

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = "compass-aristo-plugin"
    gem.summary = %Q{A Compass plugin that provides a CSS3 port of the Aristo UI elements}
    gem.description = %Q{A Compass plugin that provides a CSS3 port of the Aristo UI elements}
    gem.email = "hpoydar@gmail.com"
    gem.homepage = "http://github.com/hpoydar/compass-aristo-plugin"
    gem.authors = ["hpoydar"]
    gem.add_development_dependency "chriseppstein-compass"
    # gem is a Gem::Specification... see http://www.rubygems.org/read/chapter/20 for additional settings
  end
rescue LoadError
  puts "Jeweler (or a dependency) not available. Install it with: sudo gem install jeweler"
end

task :default => :examples

desc "Compile examples into HTML and CSS"
task :examples do
  require 'haml'
  require 'sass'
  require 'pathname'
  require 'compass'
  require 'compass/exec'
  FileList['examples/*'].each do |example|
    next unless File.directory?(example)
    puts "\nCompiling #{example}"
    puts "=" * "Compiling #{example}".length
    # compile any haml templates to html
    FileList["#{example}/**/*.haml"].each do |haml_file|
      basename = haml_file[0..-6]
      engine = Haml::Engine.new(open(haml_file).read, :filename => haml_file)
      puts "     haml #{File.basename(basename)}"
      output = open(basename,'w')
      output.write(engine.render)
      output.close
    end
    Dir.chdir example do
      Compass::Exec::Compass.new(["--force"]).run!
    end
  end
end