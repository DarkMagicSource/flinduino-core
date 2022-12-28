# flinduino-core (mac-fix)

Downloadable core for the 'Flinders Flinduino' board in Arduino IDE

## Instalation instructions

Instalation into the Arduino IDE is via the Boards Manager. Simply place this URL

https://raw.githubusercontent.com/DarkMagicSource/flinduino-core/master/package_flinduino_index.json

in the Preferences->Additional Boards Manager URLs: text field and then opening up the Boards Manager in the Tools->Board menu. 

> NOTE: you may need to force Arduino to redownload the package index, do this by running the command
`rm ~/Library/Arduino15/package_flinduino_index.json`



## Build Requirements

* [ANT](http://ant.apache.org/)

## Build Options

ant setup

ant github-release



