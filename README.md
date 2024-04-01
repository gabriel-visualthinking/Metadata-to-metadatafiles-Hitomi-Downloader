# Hitomi-Downloader-metadata-to-metadatafiles

This script automatically generates a `metadata.file` after a task is finished.

## Usage

Simply decompress the .zip file and install the `script.hds` in the Hitomi Downloader program. It is specifically designed to work with e-hentai and Hitomi websites.

## Features

- Automatically generates a `metadata.file` based on extracted metadata. Currently, it only supports the ComicInfo.xml format. (More formats will be added later)
- Places the `metadata.file` in the folder of the downloaded task for easy access.
- Transforms tags to include gender symbols for better readability. For example, "female:XX, male:XX" is transformed to "♀ XX, ♂ XX".
- Includes all metadata from the `info.txt` file in the `metadata.file`, such as "Gallery ID", "Title", "Artists", "Groups", etc.
- Adds the URL of the downloaded task to the `metadata.file`.

## Notes

- This is my first script using Python with ChatGPT.
- The ComicInfo.xml saves 'Tags' as '<Genre>', 'Group' as '<Team>', and 'Language' is converted to '<LanguageISO>' specifically to ensure compatibility with ComicRack.
- The compression option does not save the `metadata.file`; users must compress it manually.
- This script does not require the `info.txt` option to be active.
- The script may not work with "anime" files, and this functionality will not be included.
- I used the "Rename after task is finished - Add artist name" script as a base, so there might be some issues, but it functions as intended.
- Tested that it works in version 4.1 of Hitomi Downloader, as for other versions it may not work if the structure changes.
