# Privacy Policy — Gradelink to Notion

_Last updated: 2 September 2026_

**Gradelink to Notion** is a Chrome extension that copies a student's
assignments from a Gradelink parent portal into a Notion database that the
parent already owns.

## The short version

The extension has no server. There is no account to create, nothing is
collected, and nothing is sent anywhere except to the parent's own Notion
workspace, at the parent's request.

## What the extension reads

When you are on the Grades page of your Gradelink portal and you click the
extension's button, it reads the assignments shown on that page: course name,
assignment title, description, the dates the teacher entered, and any files the
teacher attached. It also reads your child's name as the portal shows it, and
the teacher's email address, which the portal publishes as a contact link on
each course.

It reads nothing else, and it reads nothing at any other time.

## Where that information goes

To one place: the Notion database you chose during setup, using the Notion
integration key you supplied. It travels directly from your browser to
`api.notion.com` over an encrypted connection.

It is not sent anywhere else. The extension contacts no other server, has no
analytics, no telemetry, no crash reporting and no third-party libraries that
phone home. There is no developer-operated server for it to talk to, because
none exists.

## What is stored on your computer

Stored locally, in the browser's extension storage, on your machine:

- Your Notion integration key.
- The identifier of the Notion database you picked.
- Your settings — children's names, subjects, courses to skip, and any personal
  assignments you added yourself.
- A record of what has already been sent, so the same assignment is not written
  twice.
- The report from the most recent run.

This is kept in `chrome.storage.local`, which stays on the device and is not
synchronised to your Google account. None of it is ever transmitted to the
developer, because there is nowhere for it to be transmitted to.

Removing the extension from Chrome deletes all of it.

## Children's information

This extension is used by parents, and the information it moves is their own
children's schoolwork. That information goes only into the parent's own Notion
workspace and is governed by the parent's Notion account. The developer has no
access to it, no copy of it, and no way to obtain it.

## What is never collected

No browsing history, no cookies, no passwords and no Gradelink login
credentials. Nothing outside the Grades page is read.

The personal details it does handle — your children's names and their teachers'
email addresses — are read only because they are part of the assignment you are
filing, and they go only into your own Notion. The developer never receives
them.

## Selling or sharing data

None of the information described here is sold, rented, shared or transferred
to anyone. This is not a policy choice that could quietly change; the extension
has no mechanism to send data to the developer at all.

## Permissions, and why each is needed

- **`storage`** — to keep your settings, your Notion key and the record of what
  has already been sent, so a second run does not duplicate the first.
- **`scripting`** — to run the reading code inside your Gradelink tab when you
  click the button. Attachments can only be fetched from inside the logged-in
  page, because they require your existing session.
- **`https://secure.gradelink.com/*`** — the assignments are read from there.
- **`https://api.notion.com/*`** — the assignments are written to there.

The extension has no permission to read any other website, and cannot.

## Changes

If this policy changes, the updated version will be posted here with a new date
at the top.

## Contact

Questions about this policy can be raised as an issue on this repository.
