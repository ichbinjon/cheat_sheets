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

---
## Dev Tools
[Sublime Text 3](https://www.sublimetext.com/3)

### Laravel

Using a Homestead VM for Laravel. Todo: learn to dockerize

[Install Docs](https://laravel.com/docs/5.5/homestead)

[VirtualBox 5.2.2](https://www.virtualbox.org/wiki/Downloads)

[Vagrant 2.0.1](https://www.vagrantup.com/downloads.html)
