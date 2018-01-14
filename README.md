komputer maschine
======

komputer maschine is a shell script that gets your machine ready for design and development.

This script can be ran once or as many times as you'd like. It installs everything that macOS needs to get to work.

## Requirements

* A komputer maschine
* macOS (>10)

## Install

```sh
curl --remote-name https://raw.githubusercontent.com/laurendorman/komputer-maschine/master/macos
sh macos 2>&1 | tee ~/komputer-maschine.log
```

## What You Get

**macOS tools:**

* [XCode Command Line Tools](https://developer.apple.com/xcode/downloads/) for developer essentials.
* [Homebrew](http://brew.sh/) for managing operating system libraries.

**Unix tools:**

* [git](https://git-scm.com/) for version control.
* [tmux](http://tmux.github.io/) for saving project state and switching between projects.
* [zsh](http://www.zsh.org/) as your shell.

**Image tools:**

* [ImageMagick](http://www.imagemagick.org/) for converting, cropping, resizing and renaming images in the command line interface.

**Programming languages and configuration:**

* [Bundler](http://bundler.io/) for managing Ruby libraries.
* [Node.js](http://nodejs.org/) and [npm](https://www.npmjs.org/) for running applications and installing JavaScript packages.
* [Rbenv](https://github.com/sstephenson/rbenv) for managing versions of Ruby.
* [Ruby Build](https://github.com/sstephenson/ruby-build) for installing Rubies.
* [Ruby](https://www.ruby-lang.org/en/) stable for writing general-purpose code.

**Applications:**

* [Alfred](https://www.alfredapp.com/) for increased productivity and efficiency with macOS.
* [Caffeine](http://lightheadsw.com/caffeine/) to keep your Mac awake.
* [Google Chrome](https://www.google.com/chrome/) for browsing the web.
* [Firefox](https://www.mozilla.org/en-US/firefox/new/) for browsing the web also, but mostly for testing. :)
* [iTerm2](https://www.iterm2.com/) for a better terminal.
* [Vagrant](https://www.vagrantup.com/) for creating and configuring development environments.
* [VirtualBox](https://www.virtualbox.org/) for guest operating systems, when needed.
* [Atom](http://atom.io) as a text editor.
* [The Unarchiver](http://unarchiver.c3.cx/unarchiver) for extracting archives that are not supported by macOS out of the box.
* [Sketch](https://www.sketchapp.com/) for design.
* [Dash](https://kapeli.com/dash) for browsing documentation and storing code snippets.
* [Slack](https://slack.com/) for more team communication and less email.
* [Docker](https://www.docker.com/) for buliding, shipping and running applications.
* [Spotify](https://www.spotify.com/us/) for music.

## Debugging

The log of your script, successful or not, will be saved to `~/komputer-maschine.log`.

Read through it to see if you can debug the issue yourself.
If not, report where the script failed into a [new GitHub Issue](https://github.com/laurendorman/komputer-maschine/issues/new).

## Known Issues

Cask does not recognize applications installed outside of Homebrew Cask – in the case that the script fails, you can either remove the application from the install list or uninstall the application causing the failure and try again.

## License

komputer maschine is © 2016 by Lauren Dorman and is protected under the [MIT License].

[MIT License]: LICENSE

## Credits and inspiration

Inspired by thoughtbot's [laptop](https://github.com/thoughtbot/laptop/) and Andrew Taylor's article on [Pantheon](https://pantheon.io/blog/dev-setup-using-homebrew-os-x).
