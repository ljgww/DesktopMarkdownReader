Desktop Markdown Reader
=====================

## Idea

Have a desktop reader application to read `.md` and `.markdown` files.

## Build it

### What you need?

1. node and npm (get it from: http://nodejs.org/)
1. node-webkit binaries (get it from: https://github.com/rogerwang/node-webkit#downloads)
1. a ZIP archiver (gets usually pre-installed on your OS, open command line and type `zip`, if you get output = you have it)
1. this source folder. Get it with git or github 'clone' command or 'Download ZIP' and expand sources 
1. markdown module (get it with: `npm install marked` shall be called from within source folder and shall create `node_modules` folder, more about marked at https://github.com/chjj/marked/) 

### How to build binary application

This requires a bit of juggling of files, but process is fairly well explained on https://github.com/rogerwang/node-webkit/wiki/How-to-package-and-distribute-your-apps 

1. zip all sources and node_modules to a .zip file
2. rename .zip file to have extension .nw (example name it `viewMarkdown.nw`)
3. follow instruction on above page to compile executable (on windows result would be `viewMarkdown.exe`)
4. copy .exe to conveniet usage dir (example windows: `c:\Program Files\Markdown Reader\`)
4. copy supporting node-webkit libraries to usage dir (on windows you need .dll and .pak files that come with node-webkit binary distribution)

### How to use reader

Once reader application is compiled to its binary form it expects one parameter - a file name. Markdown filenames are usually `.md` or `.markdown`

File name shall be specified with a full path, otherwise reader would not manage to find it as it usually runs from a temp dir (not your current work dir)

### Windows

- To read file, right click on `.md` or `.markdown file`, select 'open with...', in the dialog click browse and navigate to `viewMarkdown.exe`, select "always use this application", Click OK.
- Reader shall show you rendered text, and every next time when you double-click on `.md` or `.markdown file` it shall open reader automatically.
- Windows supplies full path name to your file
