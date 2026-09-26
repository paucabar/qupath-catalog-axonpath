# AxonPath catalog for QuPath

An extension catalog for [QuPath](https://qupath.github.io) (v0.7.0 or later) that lets you install
the [AxonPath extension](https://github.com/paucabar/qupath-extension-axonpath) from inside
QuPath and get notified when updates come out.

## Installing AxonPath

1. In QuPath, open **Extensions → Manage extensions**.
2. Click **Manage extension catalogs**.
3. Paste this URL and click **Add**:
   ```
   https://github.com/paucabar/qupath-catalog-axonpath
   ```
4. Close the catalog window. **AxonPath** now appears in the extension list; click the install
   button next to it.
5. Restart QuPath if prompted. The extension is available under **Extensions → AxonPath**.

Before running AxonPath for the first time, download the PyTorch engine: open
**Extensions → Deep Java Library → Manage DJL engines** and click **Download** next to PyTorch.
This needs an internet connection and only has to be done once.

## For maintainers

`catalog.json` follows the QuPath extension catalog format. When publishing a new AxonPath
release, add a new entry at the **top** of the `releases` list pointing to the JAR attached to
the GitHub release. All URLs must be `https` links to `github.com` (or Maven Central /
SciJava), and version names must look like `v0.1.0`.
