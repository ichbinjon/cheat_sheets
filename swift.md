# Swift Dev Cheat Sheet

## User Defaults

### Remove all information

`defaults delete your.app.bundle.id`

### Remove a specific key

`defaults delete your.app.bundle.id key`

## Cleaning DerivedData for weird build errors

`rm -rf /Users/ichbinjon/Library/Developer/Xcode/DerivedData/*`
