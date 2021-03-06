# RetroTxt

## Source code

![Code Climate](https://codeclimate.com/github/bengarrett/RetroTxt/badges/gpa.svg)

RetroTxt employs an [open sourced license](https://choosealicense.com/licenses/lgpl-3.0/) with the complete code available on [GitHub](https://github.com/bengarrett/RetroTxt). This page instructs on how to use the source in both Chrome and Firefox web browsers.

### Download

Download the RetroTxt source code onto your local computer.

Either by using [this GitHub link](https://github.com/bengarrett/RetroTxt/archive/master.zip) and decompress the saved `RetroTxt-master.zip`.

Or run the following command in a terminal.

`git clone https://github.com/bengarrett/RetroTxt.git`

### Use on Chrome

I suggest that you create a new user profile in Chrome and use that to load and edit this web extension.

1. Open a new tab and type in the address `chrome://extensions`
1. In the Extensions, tab check to enable  __Developer Mode__
1. Click the __Load unpacked extension...__ button
1. Navigate to the local directory containing the RetroTxt source code and select OK

![Font options selection](assets/sourcecode_chrome_loaded.png)

RetroTxt should load. The [Options link](options.md) allows you to configure RetroTxt styling and behaviour. You can test RetroTxt and its Options while browsing a site like [Jason Scott's Top 100 Textfiles](http://textfiles.com/100/).

### Use on Firefox

Firefox is locked down and doesn't permit the loading of extensions outside of the Mozilla Add-ons page.

Instead, there are two options to use the source code. Either use Mozilla's terminal tool `web-ext` or use [Firefox Developer Edition](https://www.mozilla.org/en-US/firefox/developer/).

The web-ext tool is the preferred method and [has a dedicated web page](https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Getting_started_with_web-ext) but requires node.js. It allows you to lint, run with options or build RetroTxt in Firefox.

1. [Install node.js if needed](https://nodejs.org)
1. `npm install --global web-ext` to install web-ext
1. `cd RetroTxt` into the cloned directory
1. `web-ext run` to run RetroTxt in Firefox
1. [Read more about web-ext](https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Getting_started_with_web-ext)

![web-ext run example](assets/web-ext_example.png)

Otherwise, if you prefer using Firefox Developer Edition.

1. Open a new tab and type in the address `about:debugging`
1. Click the __Load Temporary Add-on__ button and navigate to the local directory containing the RetroTxt source code
1. Open the `manifest.json` file to load RetroTxt

![Font options selection](assets/sourcecode_firefox.png)

Now in the same tab.

1. Type in the address `about:addons`
1. Select __Extensions__
1. RetroTxt should be listed there with some including __Options__
1. The [Options button](options.md) allows you to configure RetroTxt styling and behaviour
1. Test RetroTxt and its Options while browsing a site like [Jason Scott's Top 100 Textfiles](http://textfiles.com/100/)

![Font options selection](assets/sourcecode_firefox_addons.png)
