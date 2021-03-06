A/B-test dev setup
===

# Get started

## Prerequisits
- Node
- Yarn
- Gulp CLI

## Installation
1. Run `yarn install`
2. Install the _User Script_ from `_utils/userscript.js` in to your user script manager like Temper Monkey or Grease Monkey

## Starting development
1. Create a new folder with two files in it
  - Name them `variant.css` and `variant.js`
2. Run `gulp --proxy "https://www.google.se/"` and repace the URL with the site you are working on. **Please note** that the `--proxy` value must be the same as the actual URL (_www_ and non _www_ matters etc.), otherwise it probably will trigger a redirect.
3. Your site will open in your default browser with the URL https://localhost:9000/
4. Add query parameters to spcify the folder and file names for what you want to have incjected
  - Do so by using the form
  - Or by appending query parameters to the URL
    - `folder=example-folder-name`
    - `css=variant.css`
    - `js=variant.js`
    - _e.g._ `https://localhost:9000/?folder=example-folder-name&css=variant.css&js=variant.js`
