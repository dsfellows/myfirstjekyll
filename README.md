## My First Jekyll

This site was designed as a very simple jekyll starter for helping learning how jekyll works.

How to install this Jekyll site:

1. Follow this [Programming Historian tutorial](http://programminghistorian.org/lessons/building-static-sites-with-jekyll-github-pages#section1) to install Jekyll dependencies on your computer.

1. Follow [these instructions](http://jekyllrb.com/docs/installation/) to install Jekyll.

2. On the myfirstjekyll repository page, click "Fork" in the upper right-hand corner and select the option to fork the repo to your account. Open Github Desktop. Click File -> Clone Repository to clone myfirstjekyll onto your desktop.

3. Open Terminal and use the "cd" command to navigate into the myfirstjekyll directory that you just installed.

4. Enter the following command in your Terminal:

>bundle exec jekyll serve --watch

(You may get an error message that says "Your bundle is locked to minitest" and tells you to "Run 'bundle install' to install missing gems." If this happens, enter the command "bundle install", wait for the installation to finish, and try "bundle exec jekyll serve --watch" again.)

5. Your Terminal window should now be displaying some text ending in "Server running... press ctrl-c to stop." This means your Jekyll site should be up and running, hosted locally on your computer. Open your browser and navigate to the address "localhost:4000" to view it.
