Desktop Markdown Reader
=====================

Idea: Have a desktop reader application to read `.md` and `.markdown` files.

## Build it

### What you need?

1. node and npm (get it from: http://nodejs.org/)
1. node-webkit binaries(get it from: https://github.com/rogerwang/node-webkit#downloads)
1. a ZIP archiver (gets usually pre-installed on your OS, open command line and type `zip`, if you get output = you have it)
1. this source folder. Get it with git or github 'clone' command or 'Download ZIP' and expand sources 
1. markdown module (get it with: `npm install marked` shall be called from within source folder and shall create `node_modules` folder) 

### How to build

This requires a bit of juggling of files, but process is fairly well written on https://github.com/rogerwang/node-webkit/wiki/How-to-package-and-distribute-your-apps 