# Updating This Site

This site uses Jekyll (the Academic Pages theme) and is built automatically by GitHub Pages whenever you push to `main`. The notes below cover the edits you are most likely to make.

## Change the main page
1. Edit `_pages/about.md` – this file is published at the site root (`/`).
2. Keep the YAML front matter at the top (between the `---` lines) and edit the Markdown body below it.
3. Use standard Markdown for text and lists. If you do not need the Liquid loops that list publications or papers, you can remove or move them just like normal Markdown blocks.
4. Commit and push the change to `main`. GitHub Pages will rebuild the site; the update is live once the Actions job finishes.

## Add a news update
1. Create a Markdown file in `_news/` named `YYYY-MM-DD-slug.md` (for example `_news/2024-08-28-iclr.md`).
2. Include front matter like the example below, then add 1–2 sentences of body text after the second `---`:
   ```markdown
   ---
   title: "ICLR Attendance"
   date: 2024-08-28
   collection: news
   excerpt: "I will be in ICLR this year—reach out if you'd like to meet."
   ---
   I will be in ICLR this year and would love to connect.
   ```
3. The home page lists the 5 most recent items automatically, and the full archive lives at `/news/` (`_pages/news.md`). No further wiring is needed.
4. Commit and push to publish the update.

## Add or edit publications/papers
1. Each paper lives in `_publications/<slug>.md`. Duplicate an existing file (for example `_publications/pdmp.md`) to keep the structure, then update the values.
2. Required front-matter keys:
   - `title`: Paper title (in quotes if it has special characters).
   - `collection: publications`: Leave as-is so Jekyll groups it correctly.
   - `category`: Use `conferences`, `journals`, or `preprints` to control which list the paper appears in on the home page.
   - `date`: Use `YYYY-MM-DD`; it controls ordering.
   - `permalink`: Follow the existing style `/publication/<YYYY-MM-DD-ShortName>`.
   - Optional but recommended: `venue`, `excerpt`, `paperurl`, `slidesurl`, `github`, `author` (for the author list shown under the title).
3. Add any Markdown body below the front matter (abstract, summary, links, etc.).
4. Commit and push. The home page sections filter papers automatically based on `category`, and the `/publications/` page lists everything.

## Preview locally (optional but helpful)
1. Install dependencies once: `bundle install`.
2. Run `bundle exec jekyll serve` and open `http://localhost:4000` to see changes before pushing.
3. Stop the server with `Ctrl+C` when you are done.

## Other common tweaks
- Update the top navigation menu in `_data/navigation.yml`.
- Upload supporting files (e.g., PDFs) to the `files/` directory and reference them with relative links like `/files/filename.pdf`.

Push any committed changes to GitHub when you are ready; GitHub Pages will redeploy the site automatically.
