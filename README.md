# Vanshika's little universe

## Open it
Double-click index.html to open the website in your browser. No installation or build is needed.
For a local server, open a terminal in this folder, run `python -m http.server 8000`, then visit http://localhost:8000.

## Personalize it
Open index.html in a text editor and find `const CONTENT = {` near the bottom.
- `compliments`, `personality`, and `thoughts`: edit card titles and messages.
- `letter`: each entry is one paragraph. Edit the greeting, message, and signature here.
- `invitation`: edit the final question, button labels, both replies, and privacy note.
- `favorites`: Vanshika's momos, black, Dairy Milk, and lilies.
- `audio`: put music you can use in assets, and replace the empty string with `assets/music.mp3`. Sound starts OFF and requires a click. Without a file, the sound button stays hidden.
Other page headings and opening text are in the HTML above the content configuration. The design colours are at the beginning of the CSS in `:root`.

## Share through Vercel
1. Create a GitHub repository and upload index.html and any files in assets. No need to upload the test file or screenshots.
2. Sign in to Vercel, choose Add New Project, and import that repository.
3. Choose the Other framework preset. Leave the build command empty and use the repository root as the output directory (.).
4. Deploy and copy the resulting HTTPS address to share.
Official guide: https://vercel.com/docs/builds/configure-a-build
No deployment has been performed for you.

## Checks
Browser verification passed: all 18 reveal cards rendered; a card revealed; letter opened; both invitation replies worked; reread worked; replay reset after either reply; mobile menu opened and closed; no horizontal overflow at 390px; audio controls hidden with no configured file; reduced-motion scrolling respected; no JavaScript exceptions. JavaScript syntax also passed.
The photo gallery has been removed; the favourites section remains. Local preview screenshots are excluded from Git.
The test uses this machine's bundled Playwright and installed browser; it is not needed to run the website.
External Google Fonts and the sunset background require internet access; local font fallbacks and gradient backgrounds remain usable if they fail. No audio file was supplied, so real audio playback was not tested.
Invitation replies stay in memory on the page and reset on replay or reload. Nothing is sent or tracked.
