# rahnemon2011.github.io

The public developer website for the games by Hadi Mohammadi, served free by GitHub Pages at
<https://rahnemon2011.github.io/>.

Everything in this repository is public. Nothing secret belongs here.

## Why it exists

- **AdMob needs it.** Google checks `app-ads.txt` on the developer website named in the store
  listings. Without that file, ads in the games earn less or are not shown.
- **The stores need it.** Google Play and the App Store ask for a developer website, and the
  Google login for the private dashboard asks for a public privacy page.
- **It costs nothing.** GitHub Pages is free for a public repository.

## What is in here

| Path | What it is |
| --- | --- |
| `index.html` | Start page: one row per game with its links |
| `app-ads.txt` | The AdMob seller line for all games. Must stay at the top level |
| `cleverwick-site/` | The Cleverwick page (and the style sheet the start page shares) |
| `icons/` | Game icons used on the start page |
| `app-dashboard-privacy.html` | Privacy page for the private dashboard's Google login |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

The pages of the other games live in their own repositories and appear under the same address:
[`/nookandcranny-site/`](https://rahnemon2011.github.io/nookandcranny-site/) and
[`/arrowick-site/`](https://rahnemon2011.github.io/arrowick-site/).

## How to change it

1. Edit the files. It is plain HTML and CSS; there is no build step.
2. Commit and push to `main`. GitHub Pages publishes it within a minute or two.
3. Open the page and check it.

## Adding a new game

1. Put its icon in `icons/`.
2. Add a row to `index.html`, in the same form as the existing rows.
3. If the game uses a **new** AdMob account, add its line to `app-ads.txt`. Games on the same
   account need no change.
4. Enter `https://rahnemon2011.github.io/` as the developer website in the store listing, so
   AdMob can find `app-ads.txt`.

## Do not

- Do not rename, move or delete `app-ads.txt`.
- Do not rename the repository: the address would change and the store listings and AdMob would
  point to nothing.
- Do not make the repository private: free GitHub Pages needs it public.
