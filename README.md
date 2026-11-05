# Gain Changer: A Framework for Audio Mixing

**Live site: https://work-kelv.github.io/gain-changer/**

Gain Changer is a set of interactive guides for learning to mix a live band, from the first gain knob to a finished master. It ends with the Mix Trainer, where you mix a simulated band and get graded against what the mixing books say.

The guides were built for a church sound team, so the examples use a typical worship band: drums, bass, electric and acoustic guitar, keys, a worship leader and backing vocalists. The mixing ideas apply to any band.

## Start here

Open `index.html` and follow the guides in order, or jump to the topic you need.

| Part | Page | What it covers |
| --- | --- | --- |
| 1 | [Signal Flow & Gain Map](signal-flow.html) | The path of a sound through the desk, and how to set gain at every stage |
| 2 | [Pan & Balance Map](pan-balance.html) | Where each part sits from left to right and how loud it sits against the others, with a band builder and practice desk |
| 3 | [Magic Frequency Map](magic-frequencies.html) | What every frequency range is called on each instrument, and what to do about it |
| 4 | [Compression Map](compression-map.html) | What each book sets on the compressor for each instrument, and why |
| 5 | [Depth & Effects Map](effects-map.html) | Reverb, delay, modulation and saturation: what they do and the settings the books use |
| 6 | [Mastering Map](mastering-map.html) | Getting a finished mix ready for its listeners: level, tone, limiting and delivery |
| 7 | [Theory for the Sound Desk](desk-theory.html) | The music theory a sound engineer uses: notes, tempo, keys and song form |
| 8 | [Mix Trainer](mix-trainer.html) | Mix a simulated band in six steps, get a grade, and save a one-page report card |

## Where the content comes from

The guides are study notes drawn from these books, which go much deeper:

- *The Mixing Engineer's Handbook* by Bobby Owsinski
- *Mixing Secrets for the Small Studio* by Mike Senior
- *Mixing with Impact* by Wessel Oltheten
- *Mixing and Mastering In the Box* by Steve Savage
- *Step By Step Mixing* by Bjorgvin Benediktsson, with *56 Mix Tips for the Small Recording Studio* by Amos Clarke
- *Mixing Heavy Music* by Jordan Valeriote
- *The Bus Compression Framework* by Nathan Nyquist
- *Open Music Theory* by Mark Gotham et al. (CC BY-SA), for the theory guide

Settings are credited to their book where they appear. Anything that doesn't come from a book is labelled, including the notes for mixing in a church and the ranges the Mix Trainer fills in itself.

The practice desk and Mix Trainer are simulations. They model levels and pans with simple maths and don't process real audio.

## The team rule on panning

Where the guides suggest a pan, instruments stay inside about 80% left or right, and hard left and right are kept for reverb returns. Many seats in a church are close to one speaker, so a hard-panned part can disappear for part of the room. Book figures are still quoted as written, so you will see hard pans in the book plans.

## Running it

There is nothing to install or build. Every page is a self-contained HTML file with its images and scripts inside it, so you can double-click `index.html` or host the folder on any static web host.

Fonts load from Google Fonts. Offline, the pages fall back to system fonts and still work. Your light or dark theme choice is saved in your browser, and so is your name if you enter one on the report card. Nothing is sent anywhere.

## Publishing on GitHub Pages

1. Put these files at the root of the repository.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, then pick your main branch and the `/ (root)` folder.

The site will appear at `https://<your-username>.github.io/<repository-name>/`.

## Editing the pages

Each guide is one large HTML file holding its own styles, data and script, so most edits are made directly in that file. A few things need to stay the same on every page:

- the top navigation bar and the Previous and Next links at the bottom
- the base rules `body{margin:0}` and `[hidden]{display:none!important}`
- the shared theme setting, stored as `guide-theme`
- the `.html` file names, because the pages link to each other by name
