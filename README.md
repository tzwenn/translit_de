# Translit_DE

A functional translit keyboard layout, that lets you write in Cryllic by typing phonetically corresponding Latin characters. Sequences of one or more Latin letters are mapped into single Cyrillic ones.

You type  | Translit_DE produces
--------- | -----------
p         | п
y, j      | ы, й
ya, ja    | я, я
s         | с
sh        | ш
shh       | щ
Yazyk     | Язык
Dobro polzhalovat'! | Добро полжаловать!


The mapping is inspired by the webservice [translit.net](http://translit.net), and turns it into a OS-wide input source. Works as advertised if you know the German keyboard layout.

## Building & Installation

### OS X
	
	cp Translit-De.keylayout ~/Library/Keyboard\ Layouts/ # for your user only, or
	sudo cp Translit-De.keylayout /Library/Keyboard\ Layouts/ # For all users
	
Then log out and in again. "Translit for German Keyboard" should appear as a new input source in your keyboard settings (Language: Other).
You can edit the file using [Ukelele](http://scripts.sil.org/ukelele).

### Windows

Build the installation executables from `Translit-De.klc` using the [Microsoft Keyboard Layout Creator](https://msdn.microsoft.com/en-us/goglobal/bb964665.aspx).

**Note**: `shh` -> `щ` mapping is not handled properly. Use `w` instead.

### X-Server (Linux, BSD)

Many distros come with a great "Russian (phonetic)" layout. Use that one. My version is incomplete and inconsistent. Don't run `xkbcomp de_translit.xkb $DISPLAY`.

## Why _DE?

I use a visual German (QWERTZ) keyboard layout, and tried to immitate its functionallity. Therefore you might find the Y/Z-letters (Ы/З) swapped, as well as some special characters. Additionally I make use of Ö, Ü, and Ä to create Ё, Ю, and Э.

This is rightfully considered unappropriate for the majority of potential users out there. On the other hand it is highly appreciated by my familiy and friends, whom I ultimately strive to make happy.

I'm open for your pull requests and willing to rename this project. Or wait for another procrastination phase.

![Layout on OS X](http://i.imgur.com/OBaQ5wW.png)