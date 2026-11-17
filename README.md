<div align="center">

<img src="public/icons/icon-128.png" width="128" alt="Quick Clear logo">

# Quick Clear

Clear browser history, downloads and site data in one click, in Chrome.

[![Download](https://img.shields.io/badge/Download-Chrome-black?style=for-the-badge&logo=googlechrome)](https://github.com/Coprimal/quick-clear-chrome/releases/latest)

</div>

<div align="center">
<img src="public/screenshot.png" alt="Quick Clear popup" width="500">
</div>

## Features

- Manual clear of history, downloads or everything, for the last hour, 24 hours, 7 days, 4 weeks or all time.
- Auto clear at a set interval (minutes, hours or days).
- Site-specific cleaner: cookies and storage of the current site or of chosen domains.
- Light and dark themes. Languages: English, Vietnamese, French.
- Playground (dev only): the popup UI in a normal browser tab.

## Requirements

- Chrome (Manifest V3).
- Permissions: `browsingData`, `history`, `downloads`, `storage`, `tabs`, `alarms`, `notifications`.

## Install

1. Download the zip from [Releases](https://github.com/Coprimal/quick-clear-chrome/releases/latest) and extract it.
2. Open `chrome://extensions` and enable **Developer mode**.
3. Click **Load unpacked** and select the extracted folder (`dist/` when built from source).

## Build

```sh
npm install

# Required for screenshot generation (headless browser)
npx puppeteer browsers install chrome-headless-shell

npm run build
```

| Command                       | What it does                                   |
| ----------------------------- | ---------------------------------------------- |
| `npm run watch`               | Watch for changes and rebuild                  |
| `npm run dev`                 | UI development with hot reload                 |
| `npm run build`               | Build to `dist/` (also regenerates screenshot) |
| `npm run build:no-screenshot` | Build without regenerating the screenshot      |
| `npm run playground`          | Preview the popup UI in a browser              |
| `npm run screenshot`          | Regenerate `public/screenshot.png`             |
| `npm run version 1.1.0`       | Update version in package.json and manifest    |
| `npm run zip`                 | Create the .zip for the Chrome Web Store       |
| `npm run prettier`            | Format code                                    |
| `npm run lint`                | Run ESLint                                     |

## Author

Made by [Coprimal](https://coprimal.dev).
