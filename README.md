# Internet Radio

A responsive, single-file internet radio player that runs in a modern browser.

## Features

- Play, pause, stop, mute, and volume controls
- Search and filter the included featured stations
- Save favorites in browser local storage
- Add custom HTTP/HTTPS direct audio stream URLs
- Responsive layout for desktop and Android/mobile browsers
- No server, build step, account, or API key required

## Run locally

Open `index.html` in a modern browser. For best compatibility, serve it from a local web server or GitHub Pages.

## Publish with GitHub Pages

1. Open the repository **Settings** tab.
2. Select **Pages** in the sidebar.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch **main** and folder **/ (root)**, then save.
5. Wait for the Pages deployment to finish. GitHub will show the published site URL in the Pages section.

## Add stations

Use **Add station** in the app and enter the station name, genre, and a direct audio stream URL (for example, an HTTPS MP3 or AAC stream). A station webpage, YouTube page, or playlist page is not necessarily a playable direct stream.

Favorites and custom stations are stored in the current browser on the current device. They do not automatically sync between devices.

## Important streaming notes

- The included SomaFM stream URLs are examples; a broadcaster may change or discontinue a stream at any time.
- Some streams may be blocked by browser mixed-content rules, CORS policies, network restrictions, or broadcaster settings. Prefer HTTPS stream URLs.
- The app does not relay, record, download, or re-host audio.
- You are responsible for confirming that you have permission to publicly rebroadcast any station or music. Listening to a public stream in a personal player is not the same as obtaining rights to rebroadcast it.
- GitHub Pages hosts the website files; it does not provide an audio streaming server or a broadcast/encoder service.

## Files

- `index.html` — complete app (HTML, CSS, and JavaScript)
