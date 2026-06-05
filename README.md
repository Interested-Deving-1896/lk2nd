[update-readmes]   Mode: rewrite — migrating to template structure...
# lk2nd

[![Built with Ona](https://ona.com/build-with-ona.svg)](https://app.ona.com/#https://github.com/Interested-Deving-1896/lk2nd)

<!-- AI:start:what-it-does -->
_Description pending._
<!-- AI:end:what-it-does -->

## Architecture

<!-- AI:start:architecture -->
_Architecture documentation pending._
<!-- AI:end:architecture -->

## Install

<!-- Add installation instructions here. This section is yours — the AI will not modify it. -->

```bash
git clone https://github.com/Interested-Deving-1896/lk2nd.git
cd lk2nd
```

## Usage

lk2nd provides the standard Android fastboot protocol for flashing/booting Android boot images.

Press `Volume Down` while booting to enter Fastboot mode.
Press `Volume Up` while booting to boot into Recovery mode.

> [!TIP]
> If your stock bootloader uses the same key combinations, you need to wait a bit before
> pressing the volume keys. Usually, waiting until the screen turns on and/or the device vibrates
> should be enough to make the stock bootloader ignore the keys.

`fastboot flash lk2nd lk2nd.img` can be used to update lk2nd directly from its
fastboot interface.

> [!IMPORTANT]
> `fastboot flash boot boot.img` will flash the actual boot image with 512 KiB offset
> into the boot partition. This is done to avoid replacing lk2nd (since it is also booted from
> the boot partition).

Other fastboot commands work normally.

### Troubleshooting
If the device shows up via fastboot you can get a log file from lk2nd using
`fastboot oem log && fastboot get_staged <output-file>`, where `<output-file>`
is either some text file to write to (e.g. `output.txt`) or `/dev/stdout` to
write the log to standard output.

## Configuration

<!-- Document configuration options here. This section is yours — the AI will not modify it. -->

## CI

<!-- AI:start:ci -->
_CI documentation pending._
<!-- AI:end:ci -->

## Mirror chain

<!-- AI:start:mirror-chain -->
This repo is maintained in [`Interested-Deving-1896/lk2nd`](https://github.com/Interested-Deving-1896/lk2nd) and mirrored through:

```
Interested-Deving-1896/lk2nd  ──►  OpenOS-Project-OSP/lk2nd  ──►  OpenOS-Project-Ecosystem-OOC/lk2nd
```

Changes flow downstream automatically via the hourly mirror chain in
[`fork-sync-all`](https://github.com/Interested-Deving-1896/fork-sync-all).
Direct commits to OSP or OOC are detected and opened as PRs back to `Interested-Deving-1896`.
<!-- AI:end:mirror-chain -->

## Contributors

<!-- AI:start:contributors -->
_Contributors pending._
<!-- AI:end:contributors -->

## Origins

<!-- AI:start:origins -->
_Original project — no upstream fork._
<!-- AI:end:origins -->

## Resources

<!-- AI:start:resources -->
_No additional resource files found._
<!-- AI:end:resources -->

## License

<!-- AI:start:license -->
<!-- License not detected — add a LICENSE file to this repo. -->
<!-- AI:end:license -->
