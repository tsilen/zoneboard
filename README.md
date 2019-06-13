# Zoneboard

## Requirements
 - Chrome Browser (recent version)
 - The Zoneboard package, get it from [the releases tab](https://github.com/tsilen/zoneboard/releases).
 - redis-server (for windows see e.g. https://github.com/MicrosoftArchive/redis/releases)

## Running
  - Run zoneboard-app-win.exe / zoneboard-app-linux / zoneboard-app-macos

## Teams
- Modify team rosters in `conf/tournament.json`
- Logo files are placed under `images/teams` in .png format
- Logo filenames should be team names in lower case with all non-alphanumeric characters replaced with underscore `_`.

## Player images
- Place under `images/players` in .jpg format
- File names should match player aliases on the player cards and in the `conf/tournament.json`, but be in lower case and have all non-alphanumeric characters replaced with underscore `_`.
- Fix rotation, e.g.: remove exifdata: `exiftool -all= *.jpg`, rotate 90deg left: `mogrify -rotate "90" *.jpg`
- Above commands come with imagemagick. Feel free to use other image editors.
- E.g. if the alias on the card is `[TEAM] The player` the filename would be `_team__the_player.jpg`.

## Misc
- Game logs are saved under `gamelogs/`

## Dev Requirements
- source code has been moved to a separate private repository. Request access if needed.
- Feel free to create issues to this repo if there are any.
