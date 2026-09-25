# App-only publishing

- Website: https://maxdavemsp.github.io/dpro-control/
- Repository: https://github.com/MaxdaveMsp/dpro-control
- Pages source: `main` branch, `/docs` directory.

This public repository contains the project website, user documentation, legal notices and built app. Keep all controller source, tests, development guides and source ZIPs out of it.

For a new app release, build and test in the private development workspace. Copy only the final app ZIP into `docs/downloads/`, update the SHA-256 checksum, version labels and release notes, and review the files before committing and pushing. Upload only the app ZIP and checksum to the GitHub release.

Do not restore the earlier source-packaging script or development source into this repository. The creator retains those separately in the local development workspace.

GitHub automatically generates repository ZIP/tar archives for tags. They contain this app-distribution repository's website and build files, not the controller source.
