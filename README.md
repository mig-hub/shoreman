shoreman
========

A shell implementation of the Procfile format.

## Install

Install as a standalone.

```
curl https://raw.github.com/hecticjeff/shoreman/master/shoreman.sh -sLo ~/bin/shoreman && \
chmod 755 ~/bin/shoreman
```

To have an always up-to-date, bleeding edge, possibly broken
version available, you can use the folowing snippet in your `.bashrc`.

```shell
alias shoreman='sh -c "$(curl -fsSL https://raw.github.com/hecticjeff/shoreman/master/shoreman.sh)"'
```

## Usage

Head into a project that has a `Procfile` in it, then simply run the
`shoreman` command, it will read your Procfile, and start up the
processes it finds.

```
cd project-with-procfile
shoreman
```

## Todo

* Automatically assign a free port to processes.
* Add proper logging so it's clear what's coming from where.
* Add concurrency controls for process types.
* Support `.env` files.

## Credits

Inspired by the original [Foreman](https://github.com/ddollar/foreman)
by David Dollar (@ddollar) and [Norman](https://github.com/josh/norman) (foreman for
Node) by Josh Peek (@josh).

Copyright (c) Chris Mytton
