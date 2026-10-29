# Sport Rosters site

Landing, support, privacy, terms and accessibility pages for the Sport Rosters app, published with GitHub Pages from `main` at https://moore99.github.io/sport-rosters-site/.

## IndexNow

IndexNow tells Bing (and through it DuckDuckGo, Yahoo, Ecosia and Copilot search), Yandex, Seznam and Naver about new or changed pages. Google doesn't use it. After each successful Pages build, `.github/workflows/indexnow.yml` POSTs every page's URL to `https://api.indexnow.org/indexnow`. It's best effort: a failure only logs a warning.

The key is `0e93af240afa44c59ff8977c16ecbb66`. It's served from the key file `0e93af240afa44c59ff8977c16ecbb66.txt` at the site root and also set as `INDEXNOW_KEY` in the workflow. It's public by design, not a secret. Because the key file sits under `/sport-rosters-site/`, IndexNow only accepts URLs under that path.
