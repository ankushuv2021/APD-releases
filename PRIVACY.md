# Privacy Policy — APD Downloader and the APD browser extension

**Last updated: 26 July 2026**

## Summary

APD does not collect your data. Nothing is sent to us or to any third party.
There are no analytics, no telemetry, no accounts and no tracking. Everything
the application and the extension handle stays on your own computer.

## Who this covers

This policy covers the **APD Downloader** desktop application for Windows and
the **APD - Download Manager** browser extension, which only works alongside it.

## What the extension handles, and where it goes

The extension processes the following on your computer, and passes it only to
the APD application running locally on your own machine at `127.0.0.1:8932`:

| Data | Why | Where it goes |
|---|---|---|
| The URL of a file you download | It is the file to be downloaded | The APD app on your computer |
| The filename and file type | To save the file with the correct name | The APD app on your computer |
| The URL of the page you downloaded from | Sent as the referer; many sites reject downloads without it | The APD app on your computer |
| Cookies for the download's domain | So downloads from sites you are signed in to succeed | The APD app on your computer |
| Media stream URLs seen on the page | So you can download video you are watching | Held in browser session storage, cleared when the tab navigates or closes |
| Your file-type preferences | So you are not asked about the same type repeatedly | Your browser's local storage |

`127.0.0.1` is your own computer. This data does not travel over the internet
and is not accessible to us or anyone else.

## What we never do

- We do not collect, store or transmit your browsing history
- We do not collect personal information, credentials or payment information
- We do not sell or transfer data to third parties
- We do not use analytics, tracking pixels or advertising
- We do not run any server that receives your data

## What the extension does not read

The extension observes network requests only to identify media manifest files
(`.m3u8` and `.mpd`). It reads the request URL and the `Content-Type` response
header. It registers no blocking handler, so it cannot and does not block,
redirect, modify or read the contents of any request or response.

## Data stored on your computer

The desktop application stores the following in
`%APPDATA%\APD Downloader\` on your own machine:

- Your settings
- Your download history (filenames, source URLs, save locations)
- In-progress download state, so downloads can be resumed
- An application log

You can delete any of it at any time, and the uninstaller offers to remove all
of it. None of it is transmitted anywhere.

## Network connections the application makes

The desktop application connects to the internet only to:

1. **Download the files you ask it to download.**
2. **Check for APD updates** — a request to the GitHub Releases API. This sends
   no personal data; it is an ordinary public API request.
3. **Update its media extraction component (yt-dlp)** — a request to the public
   PyPI package index. This sends no personal data.

## Third-party components

APD bundles the open-source tools `yt-dlp`, `aria2` and `ffmpeg` to perform
downloads. They run on your computer and are governed by their own licences.

## Permissions

Every browser permission the extension requests, and the reason for it, is
listed on the Chrome Web Store listing page.

## Changes

If this policy changes, the updated version will be published here with a new
date at the top.

## Contact

Questions or concerns: https://github.com/ankushuv2021/APD/issues
