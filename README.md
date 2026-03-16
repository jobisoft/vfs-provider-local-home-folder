# The "Local Home Folder Access Provider" for the VFS Toolkit
A provider add-on for WebExtensions using the [VFS Toolkit](https://github.com/thunderbird/webext-support/tree/master/modules/vfs-toolkit), that allows WebExtensions to access the users local home folder via **native messaging**.

<p align="center">
  <img src="https://raw.githubusercontent.com/thunderbird/webext-support/refs/heads/master/modules/vfs-toolkit/vfs-toolkit-filepicker.png" alt="VFS Toolkit File Picker" width="600"><br>
  <em>Example of a VFS Toolkit file picker using the "Local Home Folder Access Provider".</em>
</p>

## Build

Set the desired version in `package.json`, then run:

```
npm run build
```

This will:
- Copy the latest `vfs-provider` library into `src/vendor/`
- Sync the version from `package.json` into `src/manifest.json`
- Update `VENDOR.md` to point to the used version
- Create `dist/vfs-toolkit-local-home-folder-access-provider.xpi` — the installable add-on
