# Project HNAR HTML5 build

Browser build for the Hello Neighbor fangame, exported from UE4.27 HTML5 (ES3/WebGL 2).

The compressed game data is split into numbered 45 MiB chunks to stay below GitHub's per-file upload limit. The UE4 loader fetches each chunk, joins them in order, decompresses the gzip stream, then hands it to the original package loader.

## Launch from a downloaded HTML file

Download [`PlayGame.html`](PlayGame.html) to your computer and open it in a current desktop browser. It loads the game files from this public repository over HTTPS, so the launcher needs an internet connection. The first launch downloads the large game data; later launches may reuse the browser's cache. Save games are stored in that browser's local storage.

For a launcher that always opens the latest published version, download [`AutoUpdate.html`](AutoUpdate.html) and open it. It redirects to the live GitHub Pages launcher, so updates appear there after they are published. Saves remain separate between the local `PlayGame.html` file and the hosted game; use the save export/import buttons to move a save between them.

You can also play from [GitHub Pages](https://masterpdiddy9.github.io/ProjectHNAR-HTML5/). This repository contains the packaged HTML5 build, not the Unreal Engine source project.
