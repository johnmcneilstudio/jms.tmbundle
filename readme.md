# Installation

**Option 1 (with Git):**
	
	mkdir -p ~/Library/Application\ Support/TextMate/Bundles/; #just in case you are missing the folder
	cd ~/Library/Application\ Support/TextMate/Bundles/;
	git clone git://github.com/johnmcneilstudio/jms.tmbundle.git "JMS.tmbundle";
	osascript -e 'tell app "TextMate" to reload bundles';
	
Installing via Git will allow you to keep up to date with the `Bundles` > `JMS` > `Update Bundle` menu command.  

**Option 2 (manual download without Git):**  
If you don't have Git and downloaded this from Github (really? you don't have Git?), after you've unzipped or untarred, you'll have to rename the folder from `johnmcneilstudio-jms.tmbundle-#{HASH}` to `JMS.tmbundle`. Double click and TextMate should install it for you.


**Option 3 (manual download via Terminal)**  
Using this method is similar to Option 2, but uses Terminal.


	mkdir -p ~/Library/Application\ Support/TextMate/Bundles
	cd ~/Library/Application\ Support/TextMate/Bundles
	wget https://github.com/johnmcneilstudio/jms.tmbundle/tarball/master
	tar zxf johnmcneilstudio-jms.tmbundle*.tar.gz
	rm johnmcneilstudio-jms.tmbundle*.tar.gz
	mv johnmcneilstudio-jms.tmbundle* JMS.tmbundle
	osascript -e 'tell app "TextMate" to reload bundles'

# Usage

**Snippets**  

| Activation Type | Activation Trigger | Scope Selector | Description |
| --------------- | ------------------ | -------------- | ----------- |
| `Tab Trigger` | `gitignore` | | Inserts our standard `.gitignore` settings |
| `Tab Trigger` | `yt` | | Inserts our standard youtube embed url with custom default parameters |

**Commands**  

| Input | Output | Activation Type | Activation Trigger | Scope Selector | Description |
| ----- | ------ | --------------- | ------------------ | -------------- | ----------- |
| `None` | `Show as HTML` | `Key Equivalent` | | | Updates the JMS TextMate Bundle via Git |


# Licenses
JMS.tmbundle is released under the MIT License. Included third-party software are limited to their respective licenses.

# Release Notes
0.0.2 (08.24.2012)

* Added Snippet for `.yt`
* Added `.yt` info to readme.md

0.0.1 (06.29.2012)

* Created JMS.tmbundle repo
* Added Snippet for `.gitignore`
* Added Command for `Update Bundle` via Git
