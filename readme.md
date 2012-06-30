# Installation

## Installation Option 1 (with Git):
	
	mkdir -p ~/Library/Application\ Support/TextMate/Bundles/; #just in case you are missing the folder
	cd ~/Library/Application\ Support/TextMate/Bundles/;
	git clone git://github.com/johnmcneilstudio/jms.tmbundle.git "JMS.tmbundle";
	osascript -e 'tell app "TextMate" to reload bundles';
	
Installing via Git will allow you to keep up to date with the `Bundles` > `JMS` > `Update Bundle` menu command.


## Installation Option 2 (manual download without GIT):
If you don't have Git and downloaded this from Github (really? you don't have Git?), after you've unzipped or untarred, you'll have to rename the folder from `johnmcneilstudio-jms.tmbundle-#{HASH}` to `JMS.tmbundle`. Double click and TextMate should install it for you.


## Installation Option 3 (manual download via Terminal)
Using this method is similar to Option 2, but uses Terminal.


	mkdir -p ~/Library/Application\ Support/TextMate/Bundles
	cd ~/Library/Application\ Support/TextMate/Bundles
	wget http://github.com/johnmcneilstudio/jms.tmbundle/tarball/master
	tar zxf jms.tmbundle*.tar.gz
	rm jms.tmbundle*.tar.gz
	mv jms.tmbundle* JMS.tmbundle
	osascript -e 'tell app "TextMate" to reload bundles'

# Usage

## Snippets

| Activation Type | Activation Trigger | Scope Selector | Description |
| --------------- | ------------------ | -------------- | ----------- |
| `Tab Trigger` | `gitignore` | | Inserts our standard `.gitignore` settings |

## Commands

| Input | Output | Activation Type | Activation Trigger | Scope Selector | Description |
| ----- | ------ | --------------- | ------------------ | -------------- | ----------- |
| `None` | `Show as HTML` | `Key Equivalent` | | | Updates the JMS TextMate Bundle via Git |


# Licenses
JMS.tmbundle is released under the MIT License. Included third-party software are limited to their respective licenses.

# Release Notes
0.0.1 (06.29.2012)

* Created JMS.tmbundle repo
* Added Snippet for `.gitignore`
* Added Command for `Update Bundle` via Git
