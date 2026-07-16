# Installation

## Download

1. Open the repository's [Releases](../../../releases) page.
2. Choose the newest non-draft release.
3. Download the macOS application archive and its checksum file.
4. Verify the download using [Verify Downloads](VERIFY_DOWNLOADS.md).
5. Move **Resolve Vector.app** into the Applications folder.

Do not download Resolve Vector from mirrors or unofficial file-sharing sites.

## First launch before notarization

Early builds may be signed locally but not yet notarized by Apple. If macOS blocks the first launch:

1. Try opening Resolve Vector once.
2. Open **System Settings → Privacy & Security**.
3. Find the message about Resolve Vector.
4. Choose **Open Anyway** and confirm.

You should only bypass this warning for a release downloaded from this repository and verified against its published checksum.

## Updates

Until automatic updates are introduced, install updates by replacing the existing application with the newer release. Your project data is stored with each project and is not removed when the application is replaced.

## Remove the application

Move **Resolve Vector.app** from Applications to the Trash. Project-specific `.vibe` directories remain in their projects unless you remove them yourself.
