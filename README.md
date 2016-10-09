# pain
Platform. API. Infrastructure. Now!

Create GDG event at one place and it will post information about it everywhere else.

## Functional specification
It's a website with two parts:

### Channels
At the top you can select various channels. Some connectors are disabled and you can enable them (by granting some permission, installing Chrome extension etc.).

Examples of channels:
- Google Developers site
- Facebook post
- Facebook event
- Meetup event
- ...

First version (MVP) needs at least two connectors.

### Form
The form is dynamically generated based on selected channels.

Some fields are required for all channels such as:
- Event title
- Event start time
- Event end time
- ...

Some fields are channel-specific such as:
- Facebook post image
- Twitter short text
- ...

After you submit the form, the information is pushed immediately to all channels.

## Project Structure

### Website
 - single form for event creation, interacts with Firebase
 - Polymer site, hosted on Firebase Hosting

### Backend
 - reacts to event creation and editation in Firebase and automates tasks via different plugins (one plugin, one file, one language = simplifies contributions)
 - AppEngine

### Browser Extension
 - because Google Dev site `sucks`, we need the extension to create and edit events on the site
 - Chrome Extension
