# Eris

> A little more momentum.

![Eris Dark](https://github.com/user-attachments/assets/27facf8e-6672-446f-971a-9a40c8d49572#gh-dark-mode-only)

![Eris Light](https://github.com/user-attachments/assets/2f64f85e-7fdc-447c-bbd1-706f12a1774d#gh-light-mode-only)

**Eris** is a native Windows download manager built for direct downloads, browser capture, media grabbing, and managing large download queues from one place.

[**Download Eris**](https://github.com/Parsa3323/Eris/releases/latest) · [Website](https://parsa3323.github.io/Eris/) · [Release history](https://github.com/Parsa3323/Eris/releases)

## Features

### Smart Split™

Smart Split dynamically divides eligible downloads into smaller byte ranges and assigns unfinished work to up to eight workers. Workers can take on remaining ranges as they become available, helping keep available connections busy.

- Uses HTTP byte-range requests when the server supports them
- Validates resource identity before resuming or assembling downloaded parts
- Supports pause, resume, retry, and recovery of unfinished downloads
- Falls back to a single connection when the server does not provide the range support or resource validation required
- Actual speed depends on the server, connection, and available network capacity

### Queues and batch downloads

- Create named queues and control how many files run at the same time
- Run up to eight active files across all queues
- Pause or resume individual downloads, a queue, or the entire app
- Generate batches from numbered URL patterns, with up to 1,000 links per batch
- Choose destinations and organize files into categories such as Programs, Compressed, Music, Videos, Documents, and Other

### Browser integration

Eris can capture direct HTTP/HTTPS downloads from supported browsers through its browser extensions and local bridge.

Supported browsers include Chrome, Edge, Opera, Brave, Vivaldi, and Firefox. Open **Settings → Browser extensions** in Eris to view the available setup options. The Firefox setup option can install the signed ErisManager add-on after the required Windows approval.

The extension also provides interception controls, including minimum file size, extension filters, domain and URL exclusions, temporary bypass, and local interception history.

### Video and audio grabbing

Enable **Grab video & audio** in the browser extension to display a download panel on supported players and embeds. Eris can offer video or audio-only downloads and lets you choose from the available video qualities.

Media handling supports direct media files and supported HLS/DASH streams. The bundled media tools support sites such as YouTube, Aparat, SoundCloud, Bandcamp, Mixcloud, and Vimeo. Availability depends on the site, player, login requirements, and available formats. DRM-protected media is not supported.

### Bandwidth and automation

- Set a global download speed limit
- Review live transfer speed and usage history
- Configure daily quotas and limits for queues, categories, and individual downloads
- Schedule bandwidth profiles
- Create automation rules triggered by events, times, or network availability
- Run queue actions and notifications, with confirmation required for external programs, scripts, and power actions

### Desktop experience

- Light, Dark, Woody, and Device themes
- Download progress, speed charts, and file-level details
- System-tray operation with controls to pause or resume downloads
- Automatic update checks and installer verification
- Download folders that can be configured by file category

## Download

The latest stable release is available from the [GitHub Releases page](https://github.com/Parsa3323/Eris/releases/latest).

For each release, the assets include the Windows installer, Chromium and Firefox extension packages, SHA-256 checksums, and the update manifest.

**Latest release:** [Eris 1.009.00](https://github.com/Parsa3323/Eris/releases/tag/v1.009.00)  
**Installer:** [Eris-Setup-1.009.00.exe](https://github.com/Parsa3323/Eris/releases/download/v1.009.00/Eris-Setup-1.009.00.exe)

## System requirements

- Windows 10 version 1809 or later, or Windows 11
- 64-bit Windows

The installer is intended for the current Windows user. Browser integration is optional and can be configured from Eris settings.

## Notes

- Smart Split needs a server that supports byte ranges and provides a usable resource validator. Eris uses a single connection when those requirements are not met.
- Browser capture requires the Eris desktop application and its local bridge to be running.
- Some websites restrict downloads or change their media delivery methods. Not every player, URL, or format can be captured.
- Authentication data is not saved in download history or queue settings.

## Links

- [Eris website](https://parsa3323.github.io/Eris/)
- [Releases and downloads](https://github.com/Parsa3323/Eris/releases)
- [Report an issue](https://github.com/Parsa3323/Eris/issues)
