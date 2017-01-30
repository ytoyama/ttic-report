require 'rake/clean'


rule '.pdf' => '.md' do |t|
  sh "pandoc -o #{t.name} #{t.source}"
end


task :view => 'notes.pdf' do
  sh 'mupdf notes.pdf'
end


task :default => 'notes.pdf'


CLEAN.include Dir.glob('*.pdf')
