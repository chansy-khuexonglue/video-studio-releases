# Video Studio

Desktop installers and automatic update files for **Video Studio**.

## Download and install

Open [the latest release](https://github.com/chansy-khuexonglue/video-studio-releases/releases/latest)
and expand **Assets** to choose your operating system.

| System | Download | Install |
| --- | --- | --- |
| Windows | `.exe` | Run the installer and follow the setup steps. |
| macOS | `.dmg` | Open the disk image and drag Video Studio into Applications. |
| Linux | `.AppImage` | Make the file executable, then run it. |

For Linux, run these commands in the download folder, replacing the filename
with the file you downloaded:

```sh
chmod +x "Video Studio-VERSION.AppImage"
./"Video Studio-VERSION.AppImage"
```

The `.tar.gz` is an alternative Linux portable build: extract it and run
`video-studio` inside the extracted folder. It requires manual updates.
If AppImage reports that FUSE is unavailable, you can extract and run it:

```sh
./"Video Studio-VERSION.AppImage" --appimage-extract
./squashfs-root/AppRun
```

## First launch

1. Open Video Studio. Without a configured API key, it opens Settings.
2. Enter your own API key in Settings and save it.
3. Create a project and choose its template and style.

Do not post API keys in this repository or its issues.

## Updates

Supported installed builds check for newer releases automatically. You can also
use **Settings → Check for updates**. Choose **Download update**, then
**Restart and install** when you are ready. Finish active video generation first.
macOS in-place updates require signed builds; portable Linux builds open the
release page for a manual download.

The `.yml` and `.blockmap` files are updater metadata. Keep them with the release
assets; users do not need to install or open them.

This repository hosts downloads and update metadata. Builds are produced by the
source repository's release workflow. If no release is listed yet, installers
have not been published.
