# Internet Radio

A responsive single-file internet radio player powered by the Radio Browser public station directory.

## Features

- Live station discovery and search using the Radio Browser API
- Genre/tag filtering and popular-station listing
- Play, pause, stop, mute, and volume controls
- Station metadata such as country, codec, and bitrate
- Radio Browser station click-counter integration when playback starts
- Save favorites and add custom direct stream URLs
- Responsive layout for desktop and Android/mobile browsers
- No API key, backend, or build step required

## API

The app uses the public Radio Browser API:
- API documentation: https://docs.radio-browser.info/
- Station search: `/json/stations/search`
- Popular stations: `/json/stations/topclick`
- Station click counter / stream resolver: `/json/url/{stationuuid}`

The app currently calls the `de1.api.radio-browser.info` API host directly from the browser. The directory is a community service and is provided without an uptime guarantee. If the service is unavailable, the live directory will show an error and can be retried with **Load stations**.

## Run locally

Open `index.html` in a modern browser. For best compatibility, serve it from a local web server or GitHub Pages.

## Publish with GitHub Pages

1. Open repository **Settings**.
2. Select **Pages** in the sidebar.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch **main** and folder **/ (root)**, then save.
5. Wait for deployment to finish. GitHub will show the published URL in the Pages section.

## Custom stations and favorites

Use **Add station** to save a station name, genre, and direct HTTP/HTTPS audio stream URL. Favorites and custom stations are stored in browser local storage on the current device; they do not sync automatically between devices.

## Streaming and rights notes

- Radio Browser is a station directory; individual stations operate their own streams.
- A station may be offline, geographically restricted, or incompatible with a particular browser.
- Prefer HTTPS streams. Browser mixed-content rules and broadcaster settings can prevent playback.
- This app plays streams for listening. It does not relay, record, download, or re-host audio.
- Public listing or personal listening does not automatically grant permission to rebroadcast music. Obtain the necessary permissions and licenses before retransmitting any station or music.
- GitHub Pages hosts website files; it is not an audio streaming server or broadcast encoder.

## Files

- `index.html` — complete app (HTML, CSS, JavaScript, and Radio Browser API integration)
