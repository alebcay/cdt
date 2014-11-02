cdt
===

Cask developer tools for Homebrew-Cask: basically the devscripts from Homebrew-Cask, but more organized

## Usage

The main executable is `cdt` on the root. Run it with any of the following subcommands:

* `hash` - give URL as argument, will download and find SHA256 sum:

```
cdt hash "https://github.com/alebcay/cdt"
```

* `help` - shows the help and list of commands
* `inspect` - view list of installed or running app or package IDs, loaded and installed launchjobs, and loaded kexts, among other things (run `cdt inspect` to view a list of things you can inspect)
* `name` - give app name as argument, will output naming scheme for your Cask:

```
cdt name "Google Chrome.app"
```

* `pkgwatch` - watch for the presence of new PKGs being installed (start observing with `cdt pkgwatch start`, and then stop observing and view results with `cdt pkgwatch stop`)
* `status` - gets the latest status information regarding which casks are failing tests (see http://github.com/alebcay/cask-tasting)
* `version` - lists version info about Cask Developer Tools.

```
cdt view vagrant
```

Thanks to the people at Homebrew-Cask, including Roland Walker, Vitor Galvao, Paul Hinze, and many others, for providing these devscripts; all I did was organize them a bit.
