# Materialminesweeper

## Description

A material(-ish) minesweeper

This is the repository for the app I am developing. The aim is to create the classic minesweeper game with a bold intentinal look using the material design concept. Also I am streaming this on livecoding.tv 

Take a look at [this link](https://www.livecoding.tv/dasheck0/videos/) for the latest livestream of this project.

## Build

In order to build the binaries you need to install gradle and run 
```
bash ./gradlew build
```
in the main directory. This will produce so called *.apk files, which can be deployed to your device. Afterwards you can deploy your apk to your device by running 
```
adb install %name%.apk
adb shell am start -n %packagename%/.MainActivity
```
In order to do this you need to install adb command line tools first.

## Features

### Game modes

Minesweeper comes in 3 classic modes
* Easy : 9x9 board with 10 bombs
* Medium : 16x16 board with 40 bombs
* Hard : 16x30 board with 99 bombs

and a new mode called expert, which has a 25x25 board with 150 bombs you need to defuse.

### History

Each game you play will be stored for you to analyse after the game. You gain such information like

* time spend to complete the game or hit the first bomb
* number of tiles revealed
* number of tiles marked

and many more. The game data as also aggregated, so that you can access average time, winning rate and many more. 

### Settings

Customize the game in every way you want. Currently you can choose, wether you want to devie to vibrate when placing flags and which backgroundmusic you want to hear while playing. There is more to come!

### Tutorial

For those who never played minesweeper there will be a tutorial, which you can swipe through when the game starts. After that you can revisit the tutorial when clicking on help in the main menu.

## Screenshot

<img src="https://github.com/dasheck0/materialminesweeper/blob/develop/art/screenshot6.png" width="240">
<img src="https://github.com/dasheck0/materialminesweeper/blob/develop/art/screenshot12.png" width="240">
<img src="https://github.com/dasheck0/materialminesweeper/blob/develop/art/screenshot2.png" width="240">
<img src="https://github.com/dasheck0/materialminesweeper/blob/develop/art/screenshot7.png" width="240">
<img src="https://github.com/dasheck0/materialminesweeper/blob/develop/art/screenshot5.png" width="240">
<img src="https://github.com/dasheck0/materialminesweeper/blob/develop/art/screenshot8.png" width="240">

# License
```
Copyright 2016 Stefan Neidig

Licensed under the GNU-GPL, Version 3.0 you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.gnu.org/licenses/gpl-3.0.txt

You may copy, distribute and modify the software as long as you track changes/dates in source files. 
Any modifications to or software including (via compiler) GPL-licensed code must also be made available 
under the GPL along with build & install instructions.
```
