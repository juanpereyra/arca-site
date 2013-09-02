def jekyll(opts="", path="")
  sh "rm -rf _site"
  sh path + "jekyll " + opts
end

desc "Build site using Jekyll"
task :build do
  jekyll
end

desc "Serve on Localhost with port 4000"
task :default do
  jekyll "serve --watch"
end

desc "Serve on Localhost with port 4000 using development version"
task :unstable do
  jekyll "serve --watch", "../jekyll/bin/"
end
