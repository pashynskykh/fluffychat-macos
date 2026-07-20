# fluffychat-macos

> **WARNING**: I’m no longer working on this project because some of the app dependencies aren’t compiling on macOS anymore.

The goal of this project is to provide a MacOS packages for the latest stable release of [FluffyChat](https://github.com/krille-chan/fluffychat). Here you'll find builds for both Apple Silicon and Intel Macs.

## Downloads

Built application can be downloaded from the [Releases](https://github.com/pashynskykh/fluffychat-macos/releases).

## Installation

1. Mount the DMG and drag and drop the app into your Applications directory.
2. Remove the "quarantine" attribute from the app:
   ```bash
   $ xattr -d com.apple.quarantine /Applications/FluffyChat.app
   ```

## FAQ

### Can I trust your builds?

My FluffyChat packages are built directly from source and I don't make any changes or even store the Fluffy Chat source code in this repository.

Also, you don't have to trust me, since you can check the `build.yml` file in this repository and make sure that it is indeed built from the original source code of the latest stable Fluffy Chat release, without any modifications.

### Why I can't open the app after installation?

If you've forgotten to remove the "quarantine" attribute, you'll receive the following message from macOS, which will prevent you from opening the application:
> Apple could not verify "FluffyChat.app" is free of malware that may harm your Mac or compromise your privacy.

This happens because I do not notarize the macOS version of the Fluffy Chat: I don't have a paid Apple Developer license and I don't want to support this signing mechanism that is put behind a paywall without providing significant gains.

### There's a new version of Fluffy Chat out. When will you update?

As soon as I manage to get some time away from work.

## License

See [LICENSE](LICENSE).
