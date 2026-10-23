# Project HNAR HTML5 build

Browser build for the Hello Neighbor fangame, exported from UE4.27 HTML5 (ES3/WebGL 2).

The compressed game data is split into numbered 45 MiB chunks to stay below GitHub's per-file upload limit. The UE4 loader fetches each chunk, joins them in order, decompresses the gzip stream, then hands it to the original package loader.

Serve `index.html` over HTTP or HTTPS (for example, GitHub Pages). This repository contains the packaged HTML5 build, not the Unreal Engine source project.