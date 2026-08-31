# ACFA HQ Command Center

Upload these three files to the same GitHub Pages repository root:

- `index.html`
- `acfa-hq-logo.jpg`
- `content.json`

## Updating Expectations, Checklist, and Notices

You no longer need to edit `index.html` to change routine staff content.

Open `content.json` in GitHub and edit the arrays:

```json
{
  "expectations": [
    "Be respectful and professional."
  ],
  "checklist": [
    "Read the latest staff announcement."
  ],
  "notices": [
    "Welcome new members and send them a cheer."
  ]
}
```

Add or remove quoted entries as needed. Keep commas between entries and make sure the JSON remains valid.

Basic HTML such as `<strong>important text</strong>` can be used inside checklist entries.

The live page requests `content.json` with cache-busting enabled so routine GitHub Pages updates should appear without editing the HTML.

## Chess.com PubAPI

`Newest Staff` still loads from Chess.com automatically.

If your HQ Chess.com club URL slug differs from:

`and-chess-for-all-hq`

update this line inside `index.html`:

```js
const CLUB_SLUG = "and-chess-for-all-hq";
```
