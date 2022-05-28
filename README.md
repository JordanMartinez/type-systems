# Type-Systems

This repo is an attempt at summarizing the main ideas behind type systems, so that I can better understand how [PureScript](https://github.com/purescript/purescript)'s type system works with the goal of improving said type system.

## License

Unless stated otherwise in a specific folder or file, this project is licensed under the `Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International license`: [(Human-readable version)](https://creativecommons.org/licenses/by-nc-sa/4.0/), [(Actual License)](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode)

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>

## Naming Conventions Used In This Repo

### Numbering System

When you see this number system:
```
01-File-Name.md
02-Folder-Name/
03-File-Name2.md
11-File-Name.md
```
You should understand it like so:
```
[major theme/idea][minor concept/point]
```
Each major theme will almost always have 1..9 minor concepts/points. Thus, you will sometimes not see a `10-file-name.md` file:
```
09-first-major-theme--file-9.md
-- 10-file-name is intentionally missing here
11-second-major-theme--file-1.md
```

In situations, where 9 files were not enough, I converted a file into a folder and each file in that folder further explains it.

### An 'x' in a File/Folder Name

If a file or folder name has `x` in the numerical part of its name (e.g. `0x-File-or-Folder-Name`, `9x-File-or-Folder-Name`), it means I am still deciding where it should appear in the numerical order (and it is likely still a work in progress).
