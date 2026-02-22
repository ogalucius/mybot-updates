[Add file] → [Create new file]
File name: README.md

Content:
# Secure Commercial Auto-Update Engine (GUI + License)

## Features
- Semantic version comparison (stable/beta channels)
- SHA256 update verification
- Automatic backup and rollback
- License key validation
- GUI progress window (Tkinter)
- Auto restart after update
- Logging system for errors & updates

## How It Works
1. Application checks stable_version.txt from GitHub.
2. Validates your license key against valid_licenses.txt.
3. If new version available, downloads zip, verifies hash, backs up old version, applies update, and restarts automatically.

## Deployment Structure
Your GitHub repository must contain:
- stable_version.txt
- stable_update.zip
- stable_hash.txt
- valid_licenses.txt

## Requirements
- Python 3.9+
- requests
- packaging
- Tkinter (built-in)

## Usage
1. Replace BASE_URL and LICENSE_KEY in updater.py
2. Run updater.py
3. GUI window shows update status

[Commit new file]
