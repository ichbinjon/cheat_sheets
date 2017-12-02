## Show hidden files and folders in Finder

```bash
defaults write com.apple.Finder AppleShowAllFiles true
killall Finder
```

## Making soft links to binary file where $PATH looks for them

```bash
ln -s /path/to/binary /usr/local/bin/binary
```

Example: Making subl open Sublime Text
```bash
ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl
```