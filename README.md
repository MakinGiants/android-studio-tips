# Android Studio Tips

List of tips for android studio

## Features
### Bookmarks
You know that you can create bookmarks to some file lines in Android Studio?

- `Ctrl + Shift + 0`: Create bookmark with 0.
- `Ctrl + Shift + 1`: Create bookmark with 1.
- `Ctrl + 0`: Go to bookmark 0.
- `Cmd + F3`: show all bookmarks.

### Selection

Word selection (like Sublible `cmd+d`):
- `Ctrl + g`: select next word with same chars.
- `Cmd + g`: skip word.

Select per block:
- `Alt + Up`: going up
- `Alt + Down`: going down

### Autocompletion
- `Cmd + space`: normal autocompletion
- `Cmd + Shift + space`: smart autocompletion (just objects with same type for ex)

## Setup 

### RAM

In Android Studio search `Help/Edit Custom VM Options` and put:

```
-XX:MaxPermSize=8G
-XX:ReservedCodeCacheSize=2G
-server

# heap - default value is 256m
-Xms4G

# Max size memory allocation pool - default value is 1280m
-Xmx4G

# defaul max value is 350m 
-XX:MetaspaceSize=4G

# use more memory but fast application.
-XX:-UseCompressedOops
```
