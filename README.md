# Git Plugin

A simple Git automation tool that scans a directory for `.git` repositories and runs `git pull`, `git push`, and `git push --tags`.

## Features

- **Directory Scanning**: Scans the specified directory for Git repositories by detecting `.git` folders.
- **Automated Git Commands**: Automatically runs the following Git commands for identified repositories:
  - `git pull`: Fetches and merges the latest changes from the remote repository.
  - `git push`: Pushes local commits to the remote repository.
  - `git push --tags`: Pushes local tags to the remote repository.
- **Command-Line Interface**: Provides a user-friendly CLI using the `click` library.

