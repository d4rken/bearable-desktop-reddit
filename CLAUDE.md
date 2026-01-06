# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Chrome extension that redirects reddit.com (and variants) to old.reddit.com using Manifest V3's declarativeNetRequest API.

## Architecture

This is a purely declarative extension with no JavaScript:

- **manifest.json** - Extension manifest (v3) with declarativeNetRequest permissions
- **rules.json** - Redirect rules using regex patterns to rewrite URLs

The extension handles these Reddit domains: `reddit.com`, `www.reddit.com`, `new.reddit.com`, `m.reddit.com`, `i.reddit.com`, `np.reddit.com`

## Development

No build step required. To test:
1. Go to `chrome://extensions/`
2. Enable "Developer mode"
3. Click "Load unpacked" and select this folder
4. After changes, click the refresh icon on the extension card
