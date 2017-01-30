require 'rake/clean'


rule '.pdf' => '.md' do |t|
  sh "pandoc -o #{t.name} #{t.source}"
end


task :default => 'notes.pdf'


CLEAN.include Dir.glob('*.pdf')
