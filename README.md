# FreshRSS - "Comics in Feed" extension

This FreshRSS extension allows you to directly comics like [The awkward yeti](https://theawkwardyeti.com/), [Buttersafe](https://www.buttersafe.com/) and more comics within your FreshRSS installation.

To use it, upload the ```freshrss-comicsinfeed``` directory to the FreshRSS `./extensions` directory on your server and enable it on the extension panel in FreshRSS.

I will probably be adding more comics in the future (when/if I start reading them) but feel free to add your own with a pull request.


## Requirements

This FreshRSS extension uses the PHP extension [DOM](http://php.net/dom) and [XML](http://php.net/xml).

As those are requirements by [FreshRSS](https://github.com/FreshRSS/FreshRSS) itself, you should be good to go.


## Installation

To install an extension, download the extension archive first and extract it on your PC (or directly on your host). Then, upload/move the folder you want on your server. Extensions must be in the ./extensions directory of your FreshRSS installation.

Then go to your FreshRSS installation and activate the extension in the extension panel - https://localhost/FreshRSS/p/i/?c=extension - and activate it.

## About FreshRSS

[FreshRSS](https://freshrss.org/) is a great self-hosted RSS Reader written in PHP, which is can also be found here at [GitHub](https://github.com/FreshRSS/FreshRSS).

More extensions can be found at [FreshRSS/Extensions](https://github.com/FreshRSS/Extensions).

## To add more comics

Essentially create a new file for your comic on the folder `./comics/` see the other files there for examples, add it to be loaded on the './comics/load.php' file and add the comic to the list of comics on the `./comics/loader.php` file.

Edit the `extension.php` file to make the match for the feed and the new function to generate the new image source.

Feel free for any pull request or to make a request for a new comic (if I have time I will add it).

## Currently supported comics

- [The awkward yeti](https://theawkwardyeti.com/)
- [Buttersafe](https://www.buttersafe.com/)
- [buni](https://www.bunicomic.com/)
- [Penny-Arcade](https://penny-arcade.com/)
- [xkcd](https://xkcd.com/)
- [Explosm](https://explosm.net/) ([RSS feed](https://explosm.net/rss.xml))
- [The Monster under the bed](https://www.themonsterunderthebed.net/)
- [Flipside](https://flipside.gushi.org) ([RSS feed](https://flipsidecomics.com/flipsiderss.php))
- [Girl Genius](https://www.girlgeniusonline.com/comic.php)
- [Questionable Content](https://questionablecontent.net/)
- [Sluggy Freelance](https://sluggy.com/)
- [Bouletcorp](https://www.bouletcorp.com/)


## Changelog

#### 1.6

4 Nov 2024

Added [Bouletcorp](https://www.bouletcorp.com/) by [SamZub](https://github.com/SamZub)


#### 1.5

2 May 2024

Added these new comics by [Joel Goguen](https://github.com/jgoguen)
- [Flipside](https://flipside.gushi.org) ([RSS feed](https://flipsidecomics.com/flipsiderss.php))
- [Girl Genius](https://www.girlgeniusonline.com/comic.php)
- [Questionable Content](https://questionablecontent.net/)
- [Sluggy Freelance](https://sluggy.com/)

#### 1.4

9 April 2024
  - Added [The Monster under the bed](https://www.themonsterunderthebed.net/) from a user request [issue #5](https://github.com/giventofly/freshrss-comicsinfeed/issues/5)

#### 1.3

14 March 2024
  - Added [Explosm](https://explosm.net/) from hidden xml rss feed thanks to [wiiaboo](https://github.com/wiiaboo)

#### 1.2

6 December 2023
  - Added [xkcd](https://xkcd.com/) images alt text, thanks to [jackson15j](https://github.com/jackson15j)
  - Penny Arcade [Penny-Arcade](https://penny-arcade.com/), thanks to [jackson15j](https://github.com/jackson15j)

#### 1.1

2 September 2023
  - Parses comics images from [buni](https://www.bunicomic.com/) feed to display fully in FreshRSS

#### 1.0

20 August 2023
 - Parses comics images from [The awkward yeti](https://theawkwardyeti.com/) feed to display fully in FreshRSS
 - Parses comics images from [Buttersafe](https://www.buttersafe.com/) feed to display fully in FreshRSS
