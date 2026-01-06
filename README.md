# Bearable Desktop Reddit

A Chrome extension that automatically redirects reddit.com to old.reddit.com because the new UI is unbearable.

## Features

- Redirects `reddit.com` → `old.reddit.com`
- Redirects `www.reddit.com` → `old.reddit.com`
- Redirects `new.reddit.com` → `old.reddit.com`
- Redirects `m.reddit.com` → `old.reddit.com`
- Redirects `i.reddit.com` → `old.reddit.com`
- Redirects `np.reddit.com` → `old.reddit.com`
- Preserves the URL path (e.g., `/r/programming` stays intact)

## Installation

1. Download or clone this repository
2. Open Chrome and go to `chrome://extensions/`
3. Enable "Developer mode" (toggle in top right)
4. Click "Load unpacked"
5. Select the folder containing this extension

## How It Works

Uses Chrome's Manifest V3 `declarativeNetRequest` API for efficient, declarative URL redirects. No background scripts running constantly - just simple redirect rules.

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.
