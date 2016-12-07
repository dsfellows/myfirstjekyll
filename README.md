## My First Jekyll

This site was designed as a very simple starter for helping learn how Jekyll works.

See below for instructions on how to install this Jekyll site. These instructions assume that:
+ You  have a Github account
+ You have [Github desktop](https://desktop.github.com/) set up on your computer
+ You have a text editor such as [Atom](https://atom.io/)
+ You have administrator privileges on the computer you're using

**Note: Jekyll is not officially supported for Windows. It should still be possible to install and run, but you may run into some difficulties. See "Troubleshooting" sections for help.**

---

1. Install Jekyll and its dependencies on your computer. You'll want to use this [Programming Historian tutorial](http://programminghistorian.org/lessons/building-static-sites-with-jekyll-github-pages#section2); start with the section titled "Installing dependencies", and stop after the tutorial tells you to run the command ```gem install jekyll```.

Note that some of the dependencies may take some time to install; even if your computer doesn't appear to be doing anything, wait until the command prompt (the thing that prompts you to type in new commands--usually your computer's name and your username, followed by a "$") reappears before typing in any new commands. This may take several minutes.

---

### Troubleshooting for Windows:

**If you get an error related to administrator privileges**, try closing Command Prompt or Git Bash then reopening it by right-clicking the program and selecting "Run as administrator."

**If you get an error message involving Ruby or Ruby's SSL, for example:**

> "ERROR: Could not find a valid gem ‘jekyll’ (>= 0), here is why:
Unable to download data from https://rubygems.org/ – SSL_connect returned=1 errno=0 state=SSLv3 read server certificate B: certificate verify failed (https://api.rubygems.org/specs.4.8.gz)"

or

> WARNING:  Unable to pull data from 'https://rubygems.org/': SSL_connect returned=1 errno=0 state=SSLv3 read server certificate B: certificate verify failed (https://api.rubygems.org/specs.4.8.gz)

Run the command ```choco upgrade ruby```, then try again.

If the command still doesn't work, try running ```gem sources --add http://rubygems.org/```.

If this doesn't work either, try appending ```--source http://rubygems.org``` to the end of the command you were initially trying to run, for example: ```gem install jekyll --source http://rubygems.org``` or ```gem install jekyll bundler --source http://rubygems.org```.

### Troubleshooting for Mac:

**If you get an error related to administrator privileges**, try adding ```sudo``` to the beginning of the command, for example: ```sudo brew install ruby```. You will need to enter your password before the command is executed. (In general, DON'T use ```sudo``` unless you're absolutely certain you understand the command you're using; it gives you access to your computer's root directory, which means you can accidentally delete important files and generally wreak havoc.)

---

2. On the myfirstjekyll repository page (the one you're on now!), click "Fork" in the upper right-hand corner and select the option to fork the repo to your Github account. Open Github Desktop. Click File -> Clone Repository to clone myfirstjekyll onto your desktop.

3. Open Terminal (on Mac) or Git Bash (on Windows) and use the ```cd``` command to navigate into the myfirstjekyll directory that you just installed.

4. Enter the following commands: ```gem install jekyll bundler```, then ```bundle install```.

5. Once the installation has finished, enter the following command:

```
bundle exec jekyll serve --watch
```

Your Terminal/Git Bash window should now be displaying some text ending in "Server running... press ctrl-c to stop." This means your Jekyll site is up and running, hosted locally on your computer. Open your browser and navigate to the address "localhost:4000" to view it.

To view the files Jekyll is using to generate your site, open the myfirstjekyll folder in Atom.

---

### Troubleshooting for Windows:

**If you get the following error, or a similar one:**

> C:/tools/ruby23/lib/ruby/gems/2.3.0/gems/bundler-1.13.6/lib/bundler/definition.rb:179:in 'rescue in specs': Your bundle is locked to RedCloth (4.2.9), but that version could not be found in any of the sources listed in your Gemfile. If you haven't changed sources, that means the author of RedCloth (4.2.9) has removed it. You'll need to update your bundle to a different version of RedCloth (4.2.9) that hasn't been removed in order to install. (Bundler::GemNotFound)

Try running ```bundle update```.

---

## Additional resources

+ See the [official Jekyll documentation](http://jekyllrb.com/docs/installation/) for more information on how to install Jekyll, check your version, update, etc. Includes tips for [how to run Jekyll on Windows](http://jekyllrb.com/docs/windows/#installation)
+ [Alternate instructions for how to install Jekyll on Windows](https://davidburela.wordpress.com/2015/11/28/easily-install-jekyll-on-windows-with-3-command-prompt-entries-and-chocolatey/), by David Burela
+ [Jekyll tutorial that explains how to use Jekyll with Github Pages](https://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages/)
