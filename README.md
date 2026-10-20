# Where to Next — team holiday poll

A one-page poll where colleagues enter their name, email, up to three ranked
destinations, preferred travel dates, budget and notes. Answers stay hidden
while the poll is open; when the organizer closes it, everyone sees:

- **Top destinations**, ranked by points (3 for a first choice, 2 for second, 1 for third)
- **Date overlap**: how many people are free each day, with the best shared window
- **Everyone's picks**, listing each person's answers

The organizer can edit or delete entries, close or reopen the poll, and download all
answers as a CSV.

## Where it runs

`holiday-wishlist.html` is published as a claude.ai Artifact:
https://claude.ai/artifact/11CJJ7rwYvPvUiG3pgF6Aw

It depends on the claude.ai Artifact runtime (`window.claude`) for its database
and for identifying the organizer, so opening the file directly or hosting it on
GitHub Pages shows the form but cannot save answers.

### Data layout

| Path | Contents |
| --- | --- |
| `responses/<email>` | One answer per email address |
| `poll/state` | `open`, `closedAt`, and a copy of the results made when the poll closes |
