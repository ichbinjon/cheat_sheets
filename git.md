
Removing files from git when adding/updating something on `.gitignore`
```
git rm -r --cached .
git add -A
git commit -am 'Removing ignored files'
```
