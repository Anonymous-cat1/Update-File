# Update File (Direct Access)
## By Anonymous_cat1, co-written by GPT-4o-Mini.

<img src="https://anonymous-cat1.github.io/Update-File/SVGassets/PMExtenGalleryThumb.svg" width="500%" height="500%"/>

### A simple Turbowarp extension that uses the [File System Access API](https://developer.mozilla.org/en-US/docs/Web/API/File_System_API) to dynamically update files.

# Security note

This will allow any Turbowarp project unrestricted access any file you specify, which means it could modify, delete, or inject something into a file without you even knowing about it!
Never allow access to files that you care about to a project you're not familiar with.

# Browser support

Your browser **must** support the File System Access API, you can find a support [list here](https://developer.mozilla.org/en-US/docs/Web/API/File_System_API#api.filesystemhandle). Otherwise, the extension will not work.
* For Firefox, you may need to install [this extension along with it's helper application](https://addons.mozilla.org/en-US/firefox/addon/file-system-access/).

# Installation
To use this extension in Turbowarp (or in it's very plentiful mods), **open Add Extension > Custom Extension** and paste this link.

**YOU MUST LOAD UNSANDBOXED. OTHERWISE IT WILL NOT IMPORT.**
```
https://anonymous-cat1.github.io/Update-File/extension.js
```
## How to use

### To start, you can open a file with the ``Set File`` block. This should open your system's file picker.

<img src="https://anonymous-cat1.github.io/Update-File/SVGassets/setfile.svg" width="100%" height="70"/>

### Now, you can update a file with the ``Write content to file from [Format Dropdown] (Text)`` block.

<img src="https://anonymous-cat1.github.io/Update-File/SVGassets/newupdatefile.svg" width="100%" height="70"/>

Dropdown options:

- Text

- URI/URL (Using a url will download whatever content the page has)

### To read a file, use the ``Get content from file as [Format Dropdown]`` reporter.

<img src="https://anonymous-cat1.github.io/Update-File/SVGassets/newgetfile.svg" width="100%" height="50"/>

Dropdown options:

- Text

- URI (always encoded as Base64)

- Hex (returns an array of bytes)

### To read a file's metedata as JSON, use the ``Get file metadata as JSON`` reporter.

<img src="https://anonymous-cat1.github.io/Update-File/SVGassets/getfilemeta.svg" width="100%" height="50"/>

### To check if a file is currentl;y opened, use the ``Is file opened?`` boolean.

<img src="https://anonymous-cat1.github.io/Update-File/SVGassets/filebool.svg" width="100%" height="50"/>

### To check if the current browser supports Direct Access (File System Access), use the ```Browser supports Direct Access?``` boolean.

<img src="https://anonymous-cat1.github.io/Update-File/SVGassets/check.svg" width="100%" height="50"/>

Lastly, to close a flie you can use ''Close File''.

<img src="https://anonymous-cat1.github.io/Update-File/SVGassets/closefile.svg" width="100%" height="70"/>
