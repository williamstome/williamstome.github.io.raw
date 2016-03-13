alias build_blog="cd ~/code/williamstome.github.io.raw; jekyll build;cp -r ~/code/williamstome.github.io.raw/_site/* ~/code/williamstome.github.io;cd ~/code/williamstome.github.io;git add .;git commit -am 'Latest build.';git push; cd ~/code/williamstome.github.io.raw"
alias bb="build_blog"
