# rahnemon2011.github.io

This is Hadi Mohammadi's free public website on GitHub Pages: <https://rahnemon2011.github.io/>.
It is the "developer website" for all of his apps and games.

Everything in this repository is public. Nothing secret belongs here.

## What the name means

GitHub Pages is GitHub's free web hosting: it turns the files of a public repository into a website.

- `github.io` is the address GitHub uses for all of these websites. Every account gets
  `https://<account name>.github.io/`.
- A repository named exactly `<account name>.github.io` is special. Each account can have only
  **one**, and it is the only one whose files appear at the **top** of that address
  (`https://rahnemon2011.github.io/app-ads.txt`).
- Every other public repository can also be a website, as many as you like, all free. Those appear
  one level down, under the repository's name: `https://rahnemon2011.github.io/arrowick-site/`.

So this repository is the front door, and the other site repositories are rooms behind it.

## Why it exists

- **AdMob needs a file at the top of the address.** Google looks for `app-ads.txt` directly under
  the developer website named in the store listings. A site one level down cannot hold it, so it
  has to be in this repository. Without the file, ads earn less or are not shown.
- **The stores ask for one developer website** for the account, not one per app. This start page
  lists every app and game with its links.
- **The private dashboard's Google login asks for a public privacy page.** It lives here too.
- **It costs nothing.**

## What is in here

| Path | What it is |
| --- | --- |
| `index.html` | Start page: one row per game with its links |
| `app-ads.txt` | The AdMob seller line for all games. Must stay at the top level |
| `cleverwick/` | One link for every device, <https://rahnemon2011.github.io/cleverwick/>: phones go to their store, computers see both buttons and a QR code. Use this one for sharing |
| `cleverwick-site/` | The Cleverwick page (and the style sheet the start page shares) |
| `icons/` | Game icons used on the start page |
| `app-dashboard-privacy.html` | Privacy page for the private dashboard's Google login |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

The pages of the other games live in their own repositories (ordinary ones, see above) and appear
under the same address:
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
- Do not rename the repository: the name is what puts it at the top of the address. Renamed, the
  store listings and AdMob would point to nothing.
- Do not make the repository private: free GitHub Pages needs it public.
