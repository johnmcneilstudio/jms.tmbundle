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

| Snippet Name | Activation Type | Activation Trigger | Scope Selector | Description |
| ------------ | --------------- | ------------------ | -------------- | ----------- |
| gitignore template | `Tab Trigger` | `gitignore` | | Inserts our standard `.gitignore` settings |
| youtube embed url | `Tab Trigger` | `yt` | | Inserts our standard youtube embed url with custom default parameters |

**Commands**  

| Command Name | Input | Output | Activation Type | Activation Trigger | Scope Selector | Description |
| ------------ | ----- | ------ | --------------- | ------------------ | -------------- | ----------- |
| Update Bundle | `None` | `Show as HTML` | `Key Equivalent` | | | Updates the JMS TextMate Bundle via Git |
| Straighten Quotes | `Selected Text` or `Document` | `Replace Selected Text` | `Key Equivalent` | | | Replaces curly single and double quotes with compatible ASCII equivalents |


# Licenses
JMS.tmbundle is released under the MIT License. Included third-party software are limited to their respective licenses.

# Release Notes
0.0.3 (09.05.2012)

* Added Command for `Straighten Quotes`
* Added `Straighten Quotes` info to readme.md

0.0.2 (08.24.2012)

* Added Snippet for `.yt`
* Added `.yt` info to readme.md

0.0.1 (06.29.2012)

* Created JMS.tmbundle repo
* Added Snippet for `.gitignore`
* Added Command for `Update Bundle` via Git
