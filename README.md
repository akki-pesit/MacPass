[![Build Status](https://travis-ci.org/mstarke/MacPass.svg?branch=continuous)](https://travis-ci.org/mstarke/MacPass)

# MacPass

There are a lot of iOS KeePass tools around but a distinct lack of a good native macOS version.
KeePass can be used via Mono on macOS but lacks vital functionality and feels sluggish and simply out of place.

MacPass is an attempt to create a native macOS port of KeePass on a solid open source foundation with a vibrant community pushing it further to become the best KeePass client for macOS.

## Download

All pre-built releases can be found at [Github](https://github.com/mstarke/MacPass/releases).

An unsigned build of the current contiuous tag can be found here: [Continuous Build](https://github.com/mstarke/MacPass/releases/tag/continuous)

Due to the nature of the build it might be unstable, however this version contains all the latest changes and bug fixes!

## How to Contribute

If you want to contribute by fixing a bug, adding a feature or improving localization you're awesome!

## How to Build

* Fetch the source of MacPass
```bash
git clone https://github.com/mstarke/MacPass --recursive
```
* Install [Carthage](https://github.com/Carthage/Carthage#installing-carthage)
* Install all Dependencies
```bash
cd MacPass
carthage bootstrap --platform macOS
```
After that you can build and run in Xcode. The following command will build and make the application available through Spotlight. If you run into signing issues take a look at [Issue #92](https://github.com/mstarke/MacPass/issues/92). Since Sparkle is disabled only on the CI build and in Debug mode, you have to explicitly disable it in Release. Otherwise warnings on unsecure updates will appear.

    xcodebuild -scheme MacPass -target MacPass -configuration Release CODE_SIGNING_REQUIRED=NO NO_SPARKLE=NO_SPARKLE

## Help

Some questions might be ansered in the [FAQ](https://github.com/mstarke/MacPass/wiki/FAQ)

Another place to look is the IRC channel [#macpass](irc://irc.freenode.org/macpass) on [irc.freenode.org](irc://irc.freenode.org)

Or follow the Twitter account [@MacPassApp](https://twitter.com/MacPassApp)

## System Requirement

The minimum macOS version required for MacPass 0.7 is 10.10 Yosemite.
The minimum OS X version required for MacPass 0.6.2 is 10.8 Mountain Lion.

## Status

The Status can be found on the dedicated [Wiki page](https://github.com/mstarke/MacPass/wiki/Status).

## What does it look like?

![image](https://raw.github.com/mstarke/MacPass/master/Assets/Screenshots/MacPass.png)

More Screenshots in the [Wiki](https://github.com/mstarke/MacPass/wiki/Screenshots)

## Alternatives
 
[KeePassX](https://www.keepassx.org) and it's fork [KeePassXC](https://github.com/keepassxreboot/keepassxc). Qt based cross plattform port.

[KyPass Companion](http://www.kyuran.be/logiciels/kypass4mac/). Native macOS client.

[KeeWeb](https://keeweb.info). Electron based cross plattform port. Since it's browser based you can pretty much run it anywhere.

## License

MacPass, a KeePass compatible Password Manager for OS X
Copyright (c) 2012-2017  Michael Starke (HicknHack Software GmbH) and all [MacPass contributors](https://github.com/mstarke/MacPass/graphs/contributors)

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of

MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.

## App Store

Due to being licensed under GPLv3 it's not possible to publish a version of MacPass on the App Store.
For further details, take a look at the [explanation](https://www.fsf.org/news/2010-05-app-store-compliance) of the Free Software Foundation.

## Contributions

The following list might not be complete, please refer to [merged Pull Requests](https://github.com/mstarke/MacPass/pulls?utf8=✓&q=is%3Apr+is%3Aclosed+is%3Amerged) on GitHub for more details. Please open an issue if you think someone is missing from this list!

### Art

[Iiro Jäppinen](https://iiro.jappinen.me) MacPass icon

[Thom Williams](https://github.com/thomscode) Document icons

[Joanna Olsen](https://github.com/JoannaOlsen) Database Icons

### Translators

[Alex Petkevich](mailto:alex@mrdoggy.info), 
[Antoine Carrincazeaux](https://github.com/AntoineCa), 
[Benjamin Steinwender](https://github.com/auge), 
[binarious](https://github.com/binarious), 
[Chester Liu](skyline75489@outlook.com), 
[Florian Gouy](https://github.com/floriangouy), 
[Francesco Servida](mailto:info@francescoservida.ch), 
[Gaétan Ryckeboer](http://gaetan.ryckeboer.org), 
[Gil André](mailto:gil@panix.com), 
[Jannick Hemelhof](https://github.com/clone1612), 
[Michał Jaglewicz](http://www.webii.pl), 
[Michel Bibal](https://github.com/MBibal), 
[Moises Perez](https://github.com/m0yP), 
[Moises Perez](https://github.com/m0yP), 
[neuroine](https://github.com/neuroine), 
[Thorsten Jacoby](https://github.com/tjacoby), 
[Volcyy](https://github.com/Volcyy), 
[Zhao Peng](mailto:patchao2000@gmail.com)

### Contributors

[Adam Doppelt](mailto:amd@gurge.com), 
[Alex Borisov](http://alexborisov.org), 
[Alex Seeholzer](https://github.com/flinz), 
[Andrew Schleifer](mailto:me@andrewschleifer.name), 
[Carlos Filipe Simões](https://github.com/ravemir), 
[Chester Liu](skyline75489@outlook.com), 
[Chhom Seng](https://github.com/cseng), 
[Christoph Leimbrock](mailto:christoph.leimbrock@gmx.de), 
[Daniele Polencic](https://github.com/danielepolencic), 
[darnel](https://github.com/darnel), 
[Deiwin Sarjas](https://github.com/deiwin), 
[Dennis Bolio](https://github.com/dennisbolio), 
[Dylan Smith](https://github.com/dylansmith), 
[Filipe Farinha](https://github.com/ktorn), 
[Frank Enderle](http://www.anamica.de/), 
[James Hurst](https://github.com/jamesrhurst), 
[Jeffrey Ying](https://github.com/Jefftree), 
[Jellyfrog](https://github.com/Jellyfrog), 
[Josh Halstead](jhalstead85@gmail.com), 
[Josh Halstead](mailto:jhalstead85@gmail.com), 
[Julian Geywitz](https://www.patreon.com/geigi), 
[Kurt Legerlotz](https://github.com/lotz), 
[lenucksi](https://github.com/lenucksi), 
[Leonardo Faoro](https://cv.lfaoro.com), 
[Liam Anderson](mailto:liam.anderson.91@gmail.com), 
[Maarten Terpstra](https://github.com/mlterpstra92), 
[Mario Sangiorgio](mailto:mariosangiorgio@gmail.com), 
[Michael Belz](https://github.com/sub0ne), 
[Nathan Landis](https://github.com/eouw0o83hf), 
[Nathaniel Madura](mailto:nmadura@umich.edu), 
[Patrik Thunström](https://github.com/magebarf), 
[rdoering](https://github.com/rdoering), 
[roasty](https://github.com/roasty), 
[Ryan Rogers](ryan@timewasted.me), 
[Sebastian Lövdahl](https://github.com/slovdahl), 
[Sitsofe Wheeler](http://sucs.org/~sits/), 
[Stephen Taylor](http://www.makegames.co.uk/), 
[thomscode](https://github.com/thomscode), 
[Thorsten Jacoby](https://github.com/tjacoby	), 
[Yono Mittlefehldt](https://twitter.com/yonomitt), 
[Zero King](https://github.com/l2dy)

## Copyright

This Project is based upon the following work:

[KeePassKit](https://github.com/mstarke/KeePassKit) Copyright 2012 HicknHack Software GmbH. All rights reserved.

[HNHUi](https://github.com/mstarke/HNHUi) Copyright 2012 HicknHack Software GmbH. All rights reserved.

[MiniKeePass](https://github.com/MiniKeePass/MiniKeePass) Copyright 2011 Jason Rush and John Flanagan. All rights reserved.

[KeePass Database Library](https://github.com/mpowrie/KeePassLib) Copyright 2010 Qiang Yu. All rights reserved.

[PXSourceList](https://github.com/Perspx/PXSourceList) Copyright 2011, Alex Rozanski. All rights reserved.

[KSPasswordField](https://github.com/karelia/SecurityInterface) Copyright 2012 Mike Abdullah, Karelia Software. All rights reserved.

[DDHotKey](https://github.com/davedelong/DDHotKey) Copyright [Dave DeLong](http://www.davedelong.com). All rights reserved.

[Sparkle](http://sparkle.andymatuschak.org) Copyright 2006 Andy Matuschak

[TransformerKit](https://github.com/mattt/TransformerKit) Licensed under MIT license. Copyright 2012 [Mattt Thompson](http://mattt.me/). All rights reserved

[MJGFoundation](https://github.com/mstarke/MJGFoundation) Licensed under BSD 2-Clause License. Copyright 2011 [Matt Galloway](http://www.galloway.me.uk/). All rights reserved.

[ShortcutRecorder](http://wafflesoftware.net/shortcut/) Copyright 2006—2013 all [Shortcut Recorder contributors](http://wafflesoftware.net/shortcut/contributors/)

[NSBundle Codesignature Check](http://jedda.me/2012/03/verifying-plugin-bundles-using-code-signing/) Copyright 2014 [Jedda Wignall](http://jedda.me). All rights reserved.

See submodules for additional Licenses

## Feedback

[![Flattr this](https://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/thing/1550529/mstarkeMacPass-on-GitHub)
