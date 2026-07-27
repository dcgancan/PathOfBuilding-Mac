# Path of Building for Mac — Patch 3.29 fix

[Path of Building](https://pathofbuilding.community/) is the build planner almost every
Path of Exile player uses. There's no official Mac version — this is a fan-made port
that runs it natively on Apple Silicon Macs, no Windows emulator needed.

**Why this fork exists:** after Patch 3.29, the official Mac port
([stevschmid/PathOfBuilding-Mac](https://github.com/stevschmid/PathOfBuilding-Mac))
fails to open — you'll see an error about a missing `sha2` module — and on some
external-monitor setups the window drew squashed into the bottom-left corner. Both are
fixed here. The fix is [already submitted](https://github.com/stevschmid/PathOfBuilding-Mac/pull/3)
upstream; this fork exists so Mac players aren't stuck waiting. **Once it's merged into
the official repo, switch back there** — this page will say so when it happens.

## Download

1. Open the **[Releases page](https://github.com/dcgancan/PathOfBuilding-Mac/releases/latest)**
   and download `PathOfBuilding-Mac.dmg`.
2. Open the downloaded file and drag **Path of Building** into your **Applications** folder.
3. Open **Applications** and double-click **Path of Building**.

### "Apple could not verify this app" / "unidentified developer"

macOS will block the first launch because this build isn't notarized by Apple (that
requires a paid Apple developer account, which this hobby project doesn't have — the
app itself is unaffected, it's the same warning you'd see for lots of small free Mac
tools). You only need to do this once:

1. Try to open the app normally — you'll get a warning dialog. Click **Done**/**Cancel**.
2. Open **System Settings → Privacy & Security**, scroll down, and you'll see
   "Path of Building was blocked...". Click **Open Anyway**.
3. Confirm in the next prompt (you may need to enter your Mac password).
4. From then on, it opens normally like any other app.

*(Screenshots of these exact steps: see [the walkthrough site](https://dcgancan.github.io/PathOfBuilding-Mac/).)*

If you'd rather not click through Settings, right-click (or Control-click) the app in
Applications, choose **Open**, then confirm **Open** in the dialog — same effect, one step.

## Requirements

- **Apple Silicon Mac** (M1, M2, M3, M4 — any "Made for Mac" chip). Intel Macs aren't supported.
- **macOS 11 (Big Sur)** or newer.
- Path of Exile 1. (This fork doesn't build the PoE2 variant — check the
  [official repo](https://github.com/stevschmid/PathOfBuilding-Mac) for that.)

## Is my data safe? Is this legit?

- It's the exact same Path of Building your Windows friends use — same build calculations,
  same passive tree, same everything — just packaged to run natively on a Mac.
  It never touches your Path of Exile account, and trading/PoE-login features work the
  same way they do on Windows (through GGG's own login page).
- All the code is public on this page. Nothing is hidden — the "Source code" link
  on the [releases page](https://github.com/dcgancan/PathOfBuilding-Mac/releases/latest)
  shows exactly what was built.
- This build is **not signed with a paid Apple certificate**, which is why you get the
  one-time warning above. It's not a virus scanner flag or malware detection — Macs
  show that warning for any app that isn't from a registered Apple developer.

## Updates

Path of Building updates its own passive tree, skills, and item data automatically —
you don't need to redownload anything for a normal game patch. You only need a new
`.dmg` from this page when the **app itself** changes (like this 3.29 fix). Check
the [Releases page](https://github.com/dcgancan/PathOfBuilding-Mac/releases) once in a
while, or just wait until something visibly breaks again.

## Found a bug?

- **Something Mac-specific** (won't open, crashes, window/graphics issues, weird
  keyboard shortcuts): [open an issue here](https://github.com/dcgancan/PathOfBuilding-Mac/issues).
  Mention your macOS version and whether you're on Apple Silicon.
- **A build/calculation looks wrong** (damage numbers, passive tree, etc.): that's the
  same on every platform — please report it to the
  [main Path of Building project](https://github.com/PathOfBuildingCommunity/PathOfBuilding/issues) instead.

## Credits

- [PathOfBuildingCommunity](https://github.com/PathOfBuildingCommunity/PathOfBuilding) —
  the actual Path of Building project this is built on top of.
- [stevschmid](https://github.com/stevschmid/PathOfBuilding-Mac) — built the original
  macOS port from scratch.
- [ocombe](https://github.com/stevschmid/PathOfBuilding-Mac/pull/3) — found and fixed
  the Patch 3.29 issues this fork carries.
- [@velomeister](https://github.com/PathOfBuildingCommunity/PathOfBuilding-SimpleGraphic/pull/98) —
  the Linux port that helped kickstart the Mac port.

## License

[MIT](https://github.com/dcgancan/PathOfBuilding-Mac/blob/master/LICENSE) for the Mac
wrapper. Path of Building itself has its own license — see
[License.md](https://github.com/PathOfBuildingCommunity/PathOfBuilding/blob/dev/LICENSE.md).
