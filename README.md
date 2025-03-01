# Wallabag v2: A TT-RSS to Wallabag v2 plugin   (Fix from @[cthu1hoo](https://github.com/cthu1hoo))

**FIX:**

**Two fixes from @[cthu1hoo](https://github.com/cthu1hoo).**

**Now the Save to Wallabag button should reappear and work again.**

**Also fix prevents plugin from being user-loaded.**










=====================
## A [TT-RSS](https://tt-rss.org/) plugin for saving links to a [Wallabag v2](https://www.wallabag.org/) instance manually or automatically via content filters.

### Installing the plugin:

#### Prepare Wallabag
1. Create a new OAuth client in the Developer tab of Wallabag and take note of the client id and client secret.
#### Prepare TT-Rss
1. Clone this repo or just grab the [latest release](https://github.com/joshp23/ttrss-to-wallabag-v2/releases/latest) and extract the wallabag_v2 folder into the `plugins.local` folder of TT-RSS v21.03-6ec66d0ce +:  
2. Install PHP Curl
	```
	sudo apt-get install php-curl
	```
3. Either enable Wallabag v2 in preferences dialogue or the TT-Rss config file
4. In TT-Rss: Simply fill in the details in the Wallabag V2 Preferences dialogue. 
5. Enjoy 1-click posting to Wallabag! (Use _Hotkeys!_ A + W )
6. Optional: Set [Content Filters](https://tt-rss.org/wiki/ContentFilters) in TT-Rss for automatic article sending to Wallabag. 

### Notes:
1. Do not add trailing slashes to any URLs in either the Wallabag or TT-Rss settings dialogues or you will get nothing but 404 responses! 
1. This plugin stores and sends Wallabag user credentials to obtain initial OAuth tokens and fetch new refresh tokens every 2 weeks as needed.
2. Set `W_V2_DEBUG` to `true` in `init.php` and a file called `debug.txt` will be created in this plugin's directory on error events. The information that is appended to that file will also appear in the developer console as it prints. This information is useful when submitting issues or trouble shooting your setup.

### TODO ... which may or not actually ever get done...
1. Add tag support
2. Add colour changing button

### Helpfull Links:
* [Official TT-RSS Plugin Documentation](https://tt-rss.org/gitlab/fox/tt-rss/wikis/Plugins)
* [Official Wallabag Documentation](http://doc.wallabag.org/en/v2/)

### Credits
Code for this project exists because of:

* [fxneumann's OneClickPocket plugin for TTRSS](https://github.com/fxneumann/oneclickpocket)
* [xppppp's Wallabag v1 plugin for TTRSS](https://github.com/xppppp/ttrss-wallabag-plugin)

### Tips
Dogecoin: DARhgg9q3HAWYZuN95DKnFonADrSWUimy3
