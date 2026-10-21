# Spell It Right

Spelling practice for college classrooms. Instructors paste a word list, check the details the app looks up, and share a link with students. There are no accounts, no database and no server. The whole list is stored inside the student link.

## How it works

- **Teacher page** (the site's main address): add words. The app fills in each word's pronunciation, definition and an example sentence from the [Free Dictionary API](https://dictionaryapi.dev/), and you can edit any of them. Then make a student link, and print or download the answer key.
- **Student link** (the same address plus `#…`): students see the pronunciation, definition and a sentence with the word blanked out. They can hear the word read aloud, and they get two tries per word. At the end they add their name and copy or download a results summary to turn in.
- **Checking results**: every summary ends with a verification code. Paste a summary into "Check a student's results" on the teacher page to confirm it hasn't been edited. This only works in the browser where you made the student link, and it deters casual edits rather than being tamper-proof.

## Deploy on GitHub Pages

1. Put `index.html` and `.nojekyll` at the root of a GitHub repository.
2. In the repository, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**, pick `main` and `/ (root)`, and select **Save**.
4. After a minute or two the site is live at `https://<your-username>.github.io/<repository-name>/`.

Everything is in the single `index.html` file. Fonts load from Google Fonts, and word lookups go to `api.dictionaryapi.dev`. Read-aloud uses the browser's built-in speech.

The live site for this repository is at https://dabush.github.io/spellitright/ once Pages is turned on.
