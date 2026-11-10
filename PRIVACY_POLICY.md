# Eris Privacy Policy

Effective date — November 5, 2026

Eris is a Windows download manager and companion browser extension developed by Parsa3323. This policy explains how they handle information when you use downloads, browser integration, media grabbing, updates, and optional features.

Developer and project contact reference — [Parsa3323 on GitHub](https://github.com/Parsa3323).

## Information used on your device

Eris processes download addresses, filenames, destination folders, file sizes, transfer progress, connection details, and error information to download and manage your files.

The desktop application stores download history, queues, recovery information, settings, schedules, automation rules, bandwidth usage, and speed-chart history locally. Its application data is normally under `%LOCALAPPDATA%\Eris\Data`. Downloaded files are stored in the folders you choose. Logs, backups, unfinished file parts, and temporary update files can also be created.

Download addresses can contain personal information, access tokens, or other confidential values. An address saved in local history retains those values as part of the address.

The browser extension stores its capture choices, media-grabbing choice, interception settings, recent interception history, and connection or error information in browser storage. Temporary media detections may be kept in session storage or local browser storage, depending on browser support.

## Browser integration and media grabbing

When Capture downloads is enabled, the extension observes download events and relevant HTTP request and response metadata to identify files and preserve their final download address. When Grab video & audio is enabled, it inspects media elements and related requests on pages to offer download controls.

For a download handed to Eris, the extension can send the following information to the Eris application on your computer through the browser's native messaging mechanism.

- The download or media address, referring page address, filename, media type, and known file size.
- Browser user-agent information and cookies associated with the requested address, when available, to support authenticated downloads.
- A request identifier and extension version for communication and compatibility checks.

Eris uses that information to make the requested download. Browser integration does not require access to the browser's saved-password database. Cookies and authentication headers are kept out of Eris's saved download queue. Media downloads can use a temporary, host-scoped cookie file, which Eris attempts to remove when the media helper finishes. An interruption can leave temporary files behind.

The extension can observe download and media metadata across websites covered by its permissions. Eris does not upload a complete browsing-history database to the developer.

## Information sent over the network

Downloading a file sends requests to its source website and any servers used for redirects or media delivery. Those servers receive the information needed for the request, such as your public IP address, requested address, user agent, and any applicable authentication context.

Eris also makes these connections when the corresponding features run.

- **Update checks and installation files.** Eris contacts GitHub and its file-delivery services for version information and update files. Requests can include the Eris version in the user agent.
- **MultiDownload connection checks.** Connection verification can contact Google's `generate_204` endpoint. Public-address checks can contact Cloudflare's trace endpoint to help distinguish network routes. Those services receive the connection's public IP address and ordinary request metadata.
- **Media downloads.** Bundled media helpers, including yt-dlp, FFmpeg, and Deno, may contact the selected media provider and its supporting servers as needed to retrieve media.
- **Browser setup and external links.** Opening an extension listing, release page, policy, or support link contacts the selected website through your browser. Your browser or extension store may separately check for extension updates.
- **Optional security scans.** When enabled, Eris asks Windows Defender to scan a file on your computer. Microsoft's cloud protection and sample-handling behavior depends on your Windows and Defender settings.

These services apply their own privacy practices. Relevant policies include [GitHub](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement), [Google](https://policies.google.com/privacy), [Cloudflare](https://www.cloudflare.com/privacypolicy/), and [Microsoft](https://privacy.microsoft.com/privacystatement).

## Developer access and optional submissions

Eris has no built-in account system, advertising analytics, or developer-operated cloud history service. Its download history and settings are kept locally instead of being routinely uploaded to the developer. Eris does not sell your personal information or use download history for advertising.

If you voluntarily send a bug report, screenshot, log, or file to the developer, that submission can contain personal information. The developer may use what you submit to respond to the request and investigate the issue. The platform through which you submit it, such as GitHub, also handles it under its own policies. Public submissions are visible to others.

## Controls and retention

You can change Capture downloads and Grab video & audio in the extension popup. Settings → Interception contains a master Enabled switch, filters, exclusions, temporary bypass, and interception-history clearing. Disabling the master switch stops supported extension capture and media handoffs while preserving your browser-specific choices.

You can also disable the extension, remove its permissions, or uninstall it. Optional security scans, MultiDownload, and automation are controlled through their settings. Closing Eris's main window can leave it running in the system tray.

Local history and settings remain until they are changed, cleared, or removed. Removing an entry changes the active history, but older backups, logs, recovery data, or temporary files can remain. Uninstallation may preserve application data. Browser storage follows the browser's retention and extension-removal behavior.

Information you submit for support is retained as needed to handle the request and meet applicable obligations, subject to the submission platform's policies. Where applicable law provides privacy rights, you may raise a request using the contact information published on the developer's GitHub profile or official extension listing. Data held by a third-party service is also subject to that service's request process.

## Security and policy changes

Eris uses the operating system's networking and storage facilities. The security of locally stored data also depends on your Windows account, device, backups, and installed software. Download sources and third-party services control their own systems.

This policy may be updated as Eris changes. The effective date above identifies the current revision. A new data use that requires permission under applicable law or browser-store rules requires the appropriate notice and permission.
