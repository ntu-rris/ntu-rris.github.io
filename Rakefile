
desc 'build the jekyll app'
task :build do
  sh "bundle exec jekyll build --trace"
end

desc 'clean _site'
task :clean do
  sh "rm -rf _site"
end

desc "bundle doctor"
task :bcheck do
  sh "bundle doctor"
end
 
desc "update bootstrap"
task :bootstrap do
  # need to do npm update or upgrade first
  sh "rsync -av node_modules/bootstrap/dist/ assets/"
  sh "rsync -av node_modules/jquery/dist/ assets/js/"
  sh "rsync -av node_modules/@popperjs/core/dist/umd/ assets/js/"
end

desc 'jekyll doctor'
task :check do
  sh "bundle exec jekyll doctor"
end

desc 'serve the jekyll app at localhost:4000'
task :start do
  sh "bundle exec jekyll serve --trace"
end

desc "default is build only"
task :default  => [ :build ]
