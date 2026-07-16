# Verify Downloads

Every public build should include a SHA-256 checksum file on its release page.

## Verify on macOS

Open Terminal in the folder containing the download and run:

```sh
shasum -a 256 "Resolve-Vector-macOS.zip"
```

Compare the complete output with the matching value published in the release's checksum file. Do not install the application if any character differs.

After extracting the application, you can inspect its signature with:

```sh
codesign --verify --deep --strict --verbose=2 "Resolve Vector.app"
```

A valid signature confirms that the bundle has not changed since it was signed. Until releases are notarized, macOS may still require the manual first-launch approval described in [Installation](INSTALLATION.md).
