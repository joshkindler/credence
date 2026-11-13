CREDENCE CHALLENGE SITE (static version)

FILES
  index.html   the whole site. You never need to edit it.
  data.json    everything visitors see (standings, outcomes, revealed forecasts, form link).
               Starts empty. You replace this one file to update the site.

PUT IT ONLINE (GitHub Pages, free)
  1. Create a GitHub account and a new public repository (e.g. "credence").
  2. Add file > Upload files: upload index.html and data.json. Commit.
  3. Settings > Pages > Source: "Deploy from a branch", Branch: main, folder: / (root). Save.
  4. After a minute or two the site is at https://YOUR-NAME.github.io/credence/
  (Netlify Drop, Cloudflare Pages, etc. also work: just upload the folder.)
  Opening index.html straight from your computer will not load data.json; it must be hosted.

ORGANIZER MODE
  Open  https://YOUR-NAME.github.io/credence/?organizer#organizer
  Only this address shows the Organizer tab. Visitors cannot change anything:
  the site only ever reads data.json. Your working data is kept in YOUR browser.
  1. Paste your Google Form link under "Submission form" > Save link.
  2. At the deadline: download the form's response sheet as CSV, choose it under
     "Import form responses", Import. Then Lock submissions, then Reveal forecasts.
  3. As statements resolve, use "Resolve questions": pick an outcome and Save.
  4. After any change: "Download data.json", then in GitHub open data.json in the repo,
     replace it (Add file > Upload files with the same name, or the pencil/edit button), Commit.
     Visitors see the update after GitHub refreshes (usually a few minutes).
  5. Now and then click "Save organizer backup" and keep that file PRIVATE
     (never put it in the repository; it contains everyone's forecasts and emails).

PRIVACY
  data.json holds only: config, outcomes, standings, and revealed forecasts for the public
  questions (and department ones if you choose). Personal answers and emails are never in it.
  Participant ids in it are one-way hashes, not emails.
