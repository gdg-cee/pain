# pain
Platform. API. Infrastructure. Now!

Create GDG event on one place and it will post information about it everywhere else.

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

Some fields are channels specific such as:
- Facebook post image
- Twitter short text
- ...

After you submit the form, the information is pushed immediately to all channels.
