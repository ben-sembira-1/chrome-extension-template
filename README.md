# chrome-extension-template
Chrome Extension Template

## Quick start
1. Decide on a name for you extension.
2. Replace all `extension_name` in the file build.yml with your chosen name.
3. Rename the directory `extension_name/` with the same name.
4. In the `manifest.json`:
   1. Give the extension a name and description.
   2. Replace the string in `matches` to a regex that represents the urls in which you want the extension to work in.
5. In the code.js add you code. If you rename the file, you should change it in `manifest.json` as well.

## CI features
1. On each push - an artifact with the current state of the extension (as crx and zip formats) will be available.
2. On each tag a release will be created (If not already created by you) with the crx and zip files as assets.
   1. The tag has to be in a valid format! 1-4 numbers separated by dots. (v1.2.3 is not valid and so as 1.0a1)
