# BSD-GAMES

This is the bsd-games package for Linux, containing classic text mode
games from UNIX folklore. `wump`, developed in 1973, `trek` from
1976 (called `spirhunt` in this version), and `adventure` from 1977,
are the oldest.

## Moved

This project has been moved to SourceForge and is not updated here.
Go to [https://sf.net/p/bsd-games](https://sf.net/p/bsd-games) for the current version.

## Installation

Installation requirements:
* C11 compiler:	gcc 4.6 or clang 3.2
* ncurses:	[https://invisible-island.net/ncurses/](https://invisible-island.net/ncurses/)
* wordlist:	for hangman. Usually already in /usr/share/dict.

```sh
./configure --prefix=/usr && make install
```

Unlike earlier bsd-games versions, this one does not install anything
sgid. Scorefiles in /var/lib/bsdgames are owned and writable by the
users group. For security, each game validates scores when loading.
Saved game files are also validated and will not cause a crash.

If you find bugs, report them on the SourceForge
[project](https://sf.net/p/bsd-games)
[bugtracker](https://sf.net/p/bsd-games/tickets).

## Included

This package contains the following games:

* adventure:	the original adventure by Crowther and Woods
* arithmetic:	asks you to do simple calculations
* atc:		air traffic control simulator
* battlestar:	a tropical adventure
* caesar:	performs rotated-alphabet cryptography (like rot13)
* cribbage:	cribbage card game
* dab:		dots and boxes
* drop4:	tetromino packing game
* gofish:	go fish card game
* gomoku:	connect-5 version of tic-tac-toe
* hangman:	guess the word before it is too late
* klondike:	curses-based solitaire
* robots:	avoid the evil robots
* sail:		sail your ship into battle
* snake:	grab the cash, avoid the snake, and exit
* spirhunt:	hunt space pirates
* worm:		eat the numbers without running into anything
* wump:		hunt the wumpus

## Excluded

Many programs that were in the original 2.17 distribution were removed
to focus on providing playable games, rather than a rusty junk pile.
boggle, mille, and monop were infringing on Hasbro copyrights. hunt,
dm, and phantasia were unplayable on single-user systems. rain and
worms were text-mode screensavers, of no use today. quiz, wtf, bcd, ppt,
morse, number, pig, pom, random, and wargames, were just plain junk.
The following programs were removed because they are already maintained
elsewhere as seprate projects.

## Found elsewhere

* backgammon:	[https://www.gnu.org/software/gnubg/](https://www.gnu.org/software/gnubg/)
* banner:	[https://packages.debian.org/stable/bsdmainutils](https://packages.debian.org/stable/bsdmainutils)
* factor:	[http://www.gnu.org/software/coreutils/coreutils.html](http://www.gnu.org/software/coreutils/coreutils.html)
* fortune:	[https://ibiblio.org/pub/linux/games/amusements/fortune/](https://ibiblio.org/pub/linux/games/amusements/fortune/)
* primes:	[http://primesieve.org/](http://primesieve.org/)
* rogue:	[http://coredumpcentral.org/](http://coredumpcentral.org/)
* hack:		[https://www.nethack.org](https://www.nethack.org), [https://github.com/msharov/hack](https://github.com/msharov/hack)
