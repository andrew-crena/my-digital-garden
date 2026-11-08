# Notes

Source for <https://andrew-crena.github.io/my-digital-garden/>: research ideas in development, and an informal journal.

| Folder | What goes in it |
| --- | --- |
| `_journal/` | Journal entries, one file per entry, named `2026-01-31-short-title.md` |
| `_ideas/` | One file per research idea, revised over time |
| `media/` | Photos, audio, and video used in either |
| `templates/` | Copy these to start an entry or an idea |

## Write a journal entry (in the browser)

1. Open [`templates/journal-entry.md`](templates/journal-entry.md), click the copy icon, and copy it.
2. Open the `_journal` folder, then **Add file → Create new file**.
3. Name it `YYYY-MM-DD-a-few-words.md`, paste, and write.
4. **Commit changes.** It stays private (`published: false`) until you change that line to `published: true`.

## Add a photo, voice memo, or video

1. Open the `media` folder, then **Add file → Upload files**, and drag the file in. Give it a short name with no spaces, like `foyer-sketch.jpg`.
2. In your entry, point to it:
   - Photo: `![What it shows](../media/foyer-sketch.jpg)`
   - Audio: `<audio controls src="../media/memo.m4a"></audio>`
   - Video: `<video controls src="../media/clip.mp4"></video>`

GitHub's upload limit is 25 MB per file. For longer recordings, upload to YouTube or SoundCloud and paste the link instead.

## Formatting cheat sheet

| Type this | To get |
| --- | --- |
| `## Heading` | A section heading |
| `*words*` | *italic* |
| `**words**` | **bold** |
| `- item` | A bulleted list |
| `> words` | A quote |
| `[text](https://...)` | A link |

## Public or private

Anything with `published: true` is on the open web. Everything in this repo, including unpublished files, can be read by anyone who opens the repo on GitHub, because the repo is public. For writing that should never be public, keep it in your Google Doc.
