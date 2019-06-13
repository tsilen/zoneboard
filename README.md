# Zoneboard

## Requirements
 - Chrome Browser (recent version)
 - redis-server (for windows see e.g. https://github.com/MicrosoftArchive/redis/releases)

## Running
  - Run zoneboard-app-win.exe / zoneboard-app-linux / zoneboard-app-macos

## Player images
- Placed under `images/players` in .jpg format
- Fix rotation, e.g.: remove exifdata: `exiftool -all= *.jpg`, rotate 90deg left: `mogrify -rotate "90" *.jpg`
- Above commands come with imagemagick
- You will need to run the build script after adding images

## Teams
- Modify team rosters in `conf/tournament.json`
- Logo files are placed under `images/teams` in .png format
- Logo filenames should be team names with all non-characters and non-digits replaced with underscore `_`

## Misc
- Game logs are saved under `gamelogs/`
- can be replayed with `node --experimental-modules backend/bin/replay-game.mjs <logfile.json>`

## Dev Requirements
- node.js 10.x (https://nodejs.org/en/)
- yarn
- source code is in a separate repo. Request access if needed.
