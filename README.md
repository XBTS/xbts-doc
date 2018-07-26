[![Build Status](https://travis-ci.org/smartholdem/api-doc.svg?branch=master)](https://travis-ci.org/smartholdem/api-doc)
[![Release](https://img.shields.io/github/release/smartholdem/api-doc.svg)](https://github.com/smartholdem/api-doc/releases/latest)

<p align="center">If you find an error in our documentation, please feel free to open up a github issue and we'll get it fixed as soon as possible.</p>

<p align="center"><img src="https://github.com/smartholdem/smartmedia/blob/master/mediakit/apiscreen.jpg" width=700 alt="Screenshot of Documentation"></p>

Getting Started
------------------------------

### Prerequisites

You're going to need:

 - **Linux or OS X** — Windows may work, but is unsupported.
 - **Ruby, version 2.3.1 or newer**
 - **Bundler** — If Ruby is already installed, but the `bundle` command doesn't work, just run `gem install bundler` in a terminal.

### Getting Set Up

1. Fork this repository on GitHub.
2. Clone *your forked repository* (not our original one) to your hard drive with `git clone https://github.com/smartholdem/api-doc.git`
3. `cd api-doc`
4. Initialize and start. You can either do this locally, or with Vagrant:

```shell

# either run this to run locally

gem install bundler
bundle install
bundle exec middleman server

# OR run this to run with vagrant

vagrant up

```

You can now see the docs at http://localhost:4567. Whoa! That was fast!

Now that Slate is all set up on your machine, you'll probably want to learn more about [editing Slate markdown](https://github.com/lord/slate/wiki/Markdown-Syntax), or [how to publish your docs](https://github.com/lord/slate/wiki/Deploying-Slate).

If you'd prefer to use Docker, instructions are available [in the wiki](https://github.com/lord/slate/wiki/Docker).

### Build

```shell

bundle exec middleman build

```

### Note on JavaScript Runtime

For those who don't have JavaScript runtime or are experiencing JavaScript runtime issues with ExecJS, it is recommended to add the [rubyracer gem](https://github.com/cowboyd/therubyracer) to your gemfile and run `bundle` again.
