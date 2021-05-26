About this mirror
=======
I don't know what has happened, but as of late May 2021 the original rsstail
author no longer appears to control the GitHub account under which rsstail
sources were hosted and developed for years. Links to vanheusden.com all appear
to be broken as well, and the original sources don't appear to survive anywhere
else on Github so far as I can tell; my old fork is now dangling off of what
appears to be a long out-of-date copy owned by someone who is not the rsstail
author. This repository contains the most recent rsstail history to which I have
access, up to date as of January 2019, and has not been intentionally modified
by me (except in one PR merged by the original author before whatever happened)
before the commit adding this section to the README.md. Unfortunately I can't
rule out random bitrot, since I can't find a copy of the original repository.

# rsstail
rsstail is tail for RSS feeds


## Usage

Basic usage:

```
rsstail -u URL -i CHECK_INTERVAL
```

For example a command below will check every 5 minutes if anything new was published:

```
$ rsstail -u http://www.filmhuisgouda.nl/rss/rss.php -i 300
Title: Que horas ela volta?
Title: 45 years
Title: Madame Bovary
...
```

`rsstail -h` will show a list of what rsstail can do for you.

## Installation

On Debian/Ubuntu:

```
sudo apt-get install rsstail
```

## Building

### Dependencies

rsstail depends on [`libmrss`](http://www.autistici.org/bakunin/codes.php#libmrss) (version >= 0.7).
On Debian/Ubuntu libmrss will be installed automatically if you install rsstail or libmrss0-dev (as shown below) as package.

To compile source code you may need to run

```
sudo apt-get install libmrss0-dev libiconv-hook-dev
```

### Compile source code

```
$ git clone https://github.com/flok99/rsstail.git
$ cd rsstail
$ sudo make install
```

## Contact

For everything more or less related to rsstail, please feel free to contact me on mail@vanheusden.com.
