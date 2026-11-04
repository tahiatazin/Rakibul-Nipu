# Rakibul Nipu – website

The official portfolio website of guitarist Rakibul Nipu.

## What's in this folder

| File / folder | What it is |
|---|---|
| `index.html` | The whole web page: all the words, plus colours and layout |
| `images/` | Every photo on the site |
| `fonts/` | The two typefaces (Anton for headings, Archivo for text) |
| `README.md` | This guide |

## Putting it online with GitHub Pages (free)

1. Sign in at github.com and click **New repository** (the **+** at the top right).
2. Give it a name, e.g. `rakibul-nipu`. Keep it **Public**. Click **Create repository**.
3. On the next page, click the link **uploading an existing file**.
4. Open this folder on your computer, select **everything inside it** (`index.html`, `images`, `fonts`, `README.md`) and drag it onto the GitHub page. Upload the contents, not the zip file.
5. Click **Commit changes**.
6. Go to **Settings → Pages**. Under **Branch**, choose `main` and `/ (root)`, then click **Save**.
7. Wait 1–2 minutes and refresh. The address appears at the top of that page, like
   `https://your-username.github.io/rakibul-nipu/`

Tip: if you name the repository `your-username.github.io`, the address is just `https://your-username.github.io`.

## Editing the words

1. In your repository, click `index.html`, then the **pencil icon** (Edit).
2. Each part of the page has a label like `===== ABOUT =====`. Use **Ctrl+F** (Cmd+F on Mac) to find the text you want.
3. Change only the words **between** the tags. For example, in
   `<p>Begins studying <strong>classical guitar</strong>.</p>`
   you can change "Begins studying" and "classical guitar", but leave `<p>`, `<strong>` etc. alone.
4. Click **Commit changes**. The live site updates within a minute or two.

### Common edits

- **Add a year to the timeline:** in the JOURNEY part, copy one whole line from `<li>` to `</li>`, paste it underneath, and change the year and text.
- **Add a song:** in the SINGLES part, copy one whole `<li> … </li>` block and change the title, year and description.
- **Change a social link:** in the SOCIAL LINKS part, change the address inside `href="…"`.

## Changing photos

**Swap a photo, keeping the same name (easiest):**
open the `images` folder on GitHub → **Add file → Upload files** → upload your new photo with **exactly the same file name** (e.g. `photo-03.webp`) → Commit. It replaces the old one.

**Use a new photo with its own name (e.g. a .jpg):**
upload it to `images`, then in `index.html` find the old file name (e.g. `images/photo-03.webp`) and change it to the new one (e.g. `images/new-gig.jpg`). File names are case-sensitive and should not contain spaces.

Keep photos under about 1 MB each so the site loads fast on phones. squoosh.app is a free tool for shrinking them.

### Which photo is where

| File | Where it appears |
|---|---|
| `hero.webp` | Opening screen (cut-out photo in front of the name) |
| `about.webp` | About section |
| `journey.webp` | Journey section |
| `bay-of-bengal.webp`, `poizon-green.webp`, `warfaze.webp` | Bands section |
| `industry-kamal.webp`, `industry-nipu.webp`, `blitz.webp`, `silversun.webp` | Collaborations section |
| `joy-bangla-concert.webp` | Live section (wide photo) |
| `photo-01.webp` … `photo-12.webp` | Photo gallery, in order |
| `torn-paper-frame.webp` | The torn-paper border around gallery photos |

## Changing colours

At the top of `index.html`, inside `<style>`, there is a block starting with `:root{`. The colours are set there:

- `--black` – page background
- `--coal` – background of the slightly lighter sections
- `--paper` – main text colour (and the light Singles section)
- `--smoke` – grey secondary text
- `--violet` – accent colour (the "Current band" label, link hover, keyboard focus)

Change a value like `#b98cf5` to any colour code. Search "colour picker" on Google to find codes.

## If something breaks

On GitHub, open `index.html` → **History** → open the last version that worked → copy it back. Every saved change is kept, so nothing is lost for good.
