Rally Print Story Cards
==============

![SCREENSHOT](https://raw.github.com/RallyApps/PrintStoryCards/master/deploy/screenshot.png)

## Overview

This Rally app shows all the stories for a given iteration in a print friendly card format. This can be used if a team wants to use a physical board to keep track of stories for an iteration.

## How to Use

### Running the App

If you want to start using the app immediately, create an Custom HTML app on your Rally dashboard. Then copy App.html from the deploy folder into the HTML text area. That's it, it should be ready to use. See [this](http://www.rallydev.com/help/use_apps#create) help link if you don't know how to create a dashboard page for Custom HTML apps.

Or you can just click [here](https://raw.github.com/RallyApps/PrintStoryCards/master/deploy/App.html) to find the file and copy it into the custom HTML app.

### Using the App

When you run this app, you can select a iteration from the drop-down list. In doing so, a list of all stories for that iteration will appear on the screen in card format. Clicking on "Print Story Cards" will open a popup window with just the story cards available for printing. This app is designed for cards to be printed in a landscape format. Make sure that landscape mode is selected when you print the cards.

<b>NOTE:</b> In Safari, you must uncheck the box "Print headers and footers". To see this option, click on the "Show Details" button on the print window. This will make sure that the cards won't overflow onto the next page, thus wasting precious paper.

## Customize this App

You're free to customize this app to your liking (see the License section for details). If you need to add any new Javascript or CSS files, make sure to update config.json so it will be included the next time you build the app.

This app uses the Rally SDK 1.32. The documentation can be found [here](http://developer.rallydev.com/help/app-sdk). 

Available Rakefile tasks are:

    rake build                      # Build a deployable app which includes all JavaScript and CSS resources inline
    rake clean                      # Clean all generated output
    rake debug                      # Build a debug version of the app, useful for local development
    rake deploy                     # Deploy an app to a Rally server
    rake deploy:debug               # Deploy a debug app to a Rally server
    rake deploy:info                # Display deploy information
    rake jslint                     # Run jslint on all JavaScript files used by this app, can be enabled by setting ENABLE_JSLINT=true.

## License

PrintStoryCards is released under the MIT license.  See the file [LICENSE](https://raw.github.com/RallyApps/PrintStoryCards/master/LICENSE) for the full text.