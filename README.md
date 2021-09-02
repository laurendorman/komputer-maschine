# komputer maschine

komputer maschine is a shell script that gets your machine ready for development.

This script can be ran once or as many times as you'd like. It installs everything that macOS needs to get to work.

## Requirements

- A komputer maschine
- macOS (>10.14)

## Install

```sh
curl --remote-name https://raw.githubusercontent.com/laurendorman/komputer-maschine/master/macos
sh macos 2>&1 | tee ~/komputer-maschine.log
```

## What You Get

**macOS tools:**

- [XCode Command Line Tools](https://developer.apple.com/xcode/downloads/) for developer essentials.
- [Homebrew](http://brew.sh/) for managing operating system libraries.

**Unix tools:**

- [git](https://git-scm.com/) for version control.
- [vim](https://www.vim.org/) for a text editor within the console.
- [tmux](http://tmux.github.io/) for saving project state and switching between projects.
- [zsh](http://www.zsh.org/) as your shell.

**Programming languages and configuration:**

- [nvm (Node Version Manager)](https://github.com/nvm-sh/nvm) and [npm](https://www.npmjs.org/) for running applications and installing JavaScript packages.
- [Python](https://www.python.org/) for programming in Python.
- [Go](https://golang.org/) for programming in Go.

**Applications:**

- [1Password](https://1password.com/) for securely managing passwords.
- [Alfred](https://www.alfredapp.com/) for increased productivity and efficiency with macOS.
- [Caffeine](http://lightheadsw.com/caffeine/) to keep your Mac awake.
- [Docker](https://www.docker.com/) for buliding, shipping and running applications.
- [Dropbox](https://www.dropbox.com/) for storing and sharing files stored in the cloud.
- [Figma](https://figma.com) for editing and viewing designs.
- [Firefox](https://www.mozilla.org/en-US/firefox/new/) for browsing the web and testing.
- [Google Chrome](https://www.google.com/chrome/) for browsing the web and testing.
- [iTerm2](https://www.iterm2.com/) for an enhanced terminal experience.
- [Loom](https://www.loom.com/) for capturing and sharing screen recordings.
- [Notion](https://www.notion.com/) for documentation, notes and task management.
- [Slack](https://slack.com/) for more team communication and less email.
- [Spotify](https://www.spotify.com/us/) for music.
- [The Unarchiver](http://unarchiver.c3.cx/unarchiver) for extracting archives that are not supported by macOS out of the box.
- [Visual Studio Code](https://code.visualstudio.com/) as an IDE.
- [Zoom](https://zoom.com/) for video calls and meetings.

## Debugging

The log of your script, successful or not, will be saved to `~/komputer-maschine.log`.

Read through it to see if you can debug the issue yourself.
If not, report where the script failed into a [new GitHub Issue](https://github.com/laurendorman/komputer-maschine/issues/new).

## Known Issues

Cask does not recognize applications installed outside of Homebrew Cask – in the case that the script fails, you can either remove the application from the install list or uninstall the application causing the failure and try again.

## License

komputer maschine is © 2016-Present by Lauren Dorman and is protected under the [MIT License].

[mit license]: LICENSE

## Credits and inspiration

Inspired by thoughtbot's [laptop](https://github.com/thoughtbot/laptop/) and Andrew Taylor's article on [Pantheon](https://pantheon.io/blog/dev-setup-using-homebrew-os-x).
