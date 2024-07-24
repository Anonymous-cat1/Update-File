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
# How to use

To start, you can open a file with the ``Set File`` block. This should open your system's file picker.

<img src="https://anonymous-cat1.github.io/Update-File/SVGassets/setfile.svg" width="100%" height="70"/>

Now, you can update a file one of two ways:
  
- 1. Plain text
  <img src="https://anonymous-cat1.github.io/Update-File/SVGassets/updatefile.svg" width="100%" height="70"/>

- 2. URI or content from a URL
  <img src="https://anonymous-cat1.github.io/Update-File/SVGassets/updatefileuri.svg" width="100%" height="70"/>

To read a file's content, you can do it also in one of two ways:
  
- 1. As Plain text
  <img src="https://anonymous-cat1.github.io/Update-File/SVGassets/getfilecon.svg" width="100%" height="70"/>

- 2. As URI
  <img src="https://anonymous-cat1.github.io/Update-File/SVGassets/getfileconasuri.svg" width="100%" height="70"/>

To read it a file's metedata as JSON, use the ``Get File Metadata`` block.

<img src="https://anonymous-cat1.github.io/Update-File/SVGassets/getfilemeta.svg" width="100%" height="70"/>

To check if the current browser supports Direct Access (File System Access) use the ''Browser supports Direct Access?'' boolean.

<img src="https://anonymous-cat1.github.io/Update-File/SVGassets/check.svg" width="100%" height="70"/>

Lastly, to close a flie you can use ''Close File''.

<img src="https://anonymous-cat1.github.io/Update-File/SVGassets/closefile.svg" width="100%" height="70"/>
