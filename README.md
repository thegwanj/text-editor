# text-editor

## Table of Contents
- [Description](#description)
- [Usage](#usage)
- [Links](#links)
- [Issues](#issues)

## Description 
Week 19 challenge where we will use our new knowledge of service workers to create an app that can store and retrieve data even if the user is offline. The following is the user story and acceptance criteria for the project:

### User Story

```md
AS A developer
I WANT to create notes or code snippets with or without an internet connection
SO THAT I can reliably retrieve them for later use
```

### Acceptance Criteria

```md
GIVEN a text editor web application
WHEN I open my application in my editor
THEN I should see a client server folder structure
WHEN I run `npm run start` from the root directory
THEN I find that my application should start up the backend and serve the client
WHEN I run the text editor application from my terminal
THEN I find that my JavaScript files have been bundled using webpack
WHEN I run my webpack plugins
THEN I find that I have a generated HTML file, service worker, and a manifest file
WHEN I use next-gen JavaScript in my application
THEN I find that the text editor still functions in the browser without errors
WHEN I open the text editor
THEN I find that IndexedDB has immediately created a database storage
WHEN I enter content and subsequently click off of the DOM window
THEN I find that the content in the text editor has been saved with IndexedDB
WHEN I reopen the text editor after closing it
THEN I find that the content in the text editor has been retrieved from our IndexedDB
WHEN I click on the Install button
THEN I download my web application as an icon on my desktop
WHEN I load my web application
THEN I should have a registered service worker using workbox
WHEN I register a service worker
THEN I should have my static assets pre cached upon loading along with subsequent pages and static assets
WHEN I deploy to Heroku
THEN I should have proper build scripts for a webpack application
```

## Usage
When launched, the user is met with a text editor. They may edit text, which is automatically saved when the user clicks out of the window, or presses the "Install" button. If the user refreshes or exits and comes back to the page, the saved text will come back and the user can pick up where they left off.

## Links
Heroku App: https://just-another-jate.herokuapp.com/

GitHub Repo: https://github.com/thegwanj/text-editor

## Issues
There is a current known issue where the install button will not actually install the app. However, up in the address bar, there is an option to install the app there. Once installed, the app functions as expected.
