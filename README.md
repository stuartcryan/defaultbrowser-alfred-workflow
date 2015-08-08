# defaultbrowser-alfred-workflow
A simple workflow to allow quick and easy changing of the default browser on OSX using a workflow in Alfred.

## Installation

1. Download the .alfredworkflow file
2. Run to import into Alfred

## Usage

* db < browser >
* Note - if you try to set the default browser that is already active as the default you will just get a notification.

Browsers currently supported:
* Chrome
* Firefox
* Opera
* Safari
* Chromium - New in V1.1
* Canary - New in V1.1
* SeaMonkey - New in V1.1

## Troubleshooting

If you are finding that you are seeing browsers listed that you have installed previously but no longer have on your system you will need to clear out all your default handlers.

Unfortunately, this is the only solution I have found to date, you should research it in depth before you use it. The following command will re-initialise all the "handlers" OSX knows about and will therefore resolve the issue, it will also likely require you to set up all your custom file associations again.

In other words... you do this at your own risk, I do not support this in any way shape or form...

The command you will need to run on the terminal is:
lsregister -kill

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Change Log

* Version 1.1 - Feature Release
	* Feature: Support additional browsers - added Chromium, Canary and SeaMonkey
	* Feature: Only show installed browsers
	* Feature: Indicate which browser is the current default
	* Feature: Added hotkey assignments (to launch workflow, launch with "chrome", and launch with "safari")
	* Improvement: Renamed description in Alfred to simply "Default Browser"
	* Improvement: Improved failure feedback
	* Improvement: Major code refactor to remove duplication and speed up the workflow
	* Improvement: Added  an icon to the workflow
	* Improvement: defaultbrowser binary has been updated to better support integrating. This code has been put into a pull request for the official publication of defaultbrowser.
* Version 1.0 - Initial Release

## Credits

[defaultbrowser binary for OSX](https://github.com/kerma/defaultbrowser) has been created by [Margus Kerma](https://github.com/kerma).
* Margus has been kind enough to permit me to include the binary for defaultbrowser as part of this workflow to make distribution significantly easier.
* For any issues with the defaultbrowser binary please log these to the official [DefaultBrowser Issue Tracker](https://github.com/kerma/defaultbrowser).

DefaultBrowser Alfred workflow created by [Stuart Ryan](http://stuartryan.com). If you would like to get into contact you can do so via:
* [@StuartCRyan on Twitter](http://twitter.com/stuartcryan)
* [Stuart Ryan on LinkedIn](https://au.linkedin.com/in/stuartcryan)
* [Technical Notebook Blog](http://technicalnotebook.com)
* [Technical Notebook Wiki](http://technicalnotebook.com/wiki)
* [Technical Notebook JIRA](http://technicalnotebook.com/jira)

## License

Released under the GNU GENERAL PUBLIC LICENSE Version 2, June 1991