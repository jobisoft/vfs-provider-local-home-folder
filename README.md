# Local Home Folder Access Provider
A VFS provider add-on that enables WebExtensions using the [VFS Toolkit](https://github.com/thunderbird/webext-support/tree/master/modules/vfs-toolkit) to access the user's local home folder through a **native messaging** helper application.

<p align="center">
  <img src="https://raw.githubusercontent.com/thunderbird/webext-support/refs/heads/master/modules/vfs-toolkit/vfs-toolkit-filepicker.png" alt="VFS Toolkit File Picker" width="600"><br>
  <em>Example of a VFS Toolkit file picker using the "Local Home Folder Access Provider".</em>
</p>

## Test

To test this provider, install the `vfs-toolkit-example-client.xpi` file from the [VFS-Toolkit](https://github.com/thunderbird/webext-support/tree/master/modules/vfs-toolkit), and the `vfs-provider-home-folder-access.xpi` file from the [latest release](https://github.com/jobisoft/vfs-provider-local-home-folder/releases) of the local home folder provider add-on.

## Build

Set the desired version in `package.json`, then run:

```
npm run build
```

This will:
- Copy the latest `vfs-provider` library into `src/vendor/`
- Sync the version from `package.json` into `src/manifest.json`
- Update `VENDOR.md` to point to the used version
- Create `dist/vfs-provider-home-folder-access.xpi` — the installable add-on
