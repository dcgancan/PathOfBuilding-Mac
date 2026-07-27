# Path of Building for Mac (updated for 3.29)

Wanted to get back into PoE with patch 3.29 and couldn't find a working, up-to-date
[Path of Building](https://pathofbuilding.community/) for Mac. Tweaked
[stevschmid's Mac port](https://github.com/stevschmid/PathOfBuilding-Mac) a bit to get it
updated and working again, so sharing it here in case it's useful to someone else.
Already sent the fix upstream too ([PR #3](https://github.com/stevschmid/PathOfBuilding-Mac/pull/3)),
so hopefully this fork won't be needed for long.

## Download

1. Grab `PathOfBuilding-Mac.dmg` from the
   **[latest release](https://github.com/dcgancan/PathOfBuilding-Mac/releases/latest)**.
2. Open the DMG and drag **Path of Building** into your Applications folder.
3. Open it from Applications.

### "Apple could not verify this app"

This build isn't notarized (no paid Apple developer account), so macOS will warn you the
first time you open it. Right-click (or Control-click) the app in Applications, choose
**Open**, then confirm **Open** again in the dialog. You only need to do this once — see
the [walkthrough](https://dcgancan.github.io/PathOfBuilding-Mac/) if you want screenshots.

## Requirements

- Apple Silicon Mac (M1 or newer). Intel isn't supported.
- macOS 11 (Big Sur) or newer.
- Path of Exile 1 — no PoE2 build here, see the
  [official repo](https://github.com/stevschmid/PathOfBuilding-Mac) for that.

## Feedback

Something works fine on Windows but not here, or something's just off on Mac (won't open,
crashes, graphics glitches)? Open an
[issue](https://github.com/dcgancan/PathOfBuilding-Mac/issues) — happy to take a look.
A build/calculation issue isn't Mac-specific, so that's better reported to the
[main Path of Building project](https://github.com/PathOfBuildingCommunity/PathOfBuilding/issues) instead.

## Credits

- [PathOfBuildingCommunity](https://github.com/PathOfBuildingCommunity/PathOfBuilding) for
  Path of Building itself.
- [stevschmid](https://github.com/stevschmid/PathOfBuilding-Mac) for the original Mac port.
- [@velomeister](https://github.com/PathOfBuildingCommunity/PathOfBuilding-SimpleGraphic/pull/98) —
  the Linux port that helped kickstart the Mac port.

## License

[MIT](https://github.com/dcgancan/PathOfBuilding-Mac/blob/master/LICENSE) for the Mac
wrapper. Path of Building itself has its own license — see
[License.md](https://github.com/PathOfBuildingCommunity/PathOfBuilding/blob/dev/LICENSE.md).
