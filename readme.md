# SPA Boilerplate

Starter project files for making single-page applications on a traditional LAMP server.

It contains a service worker (`/sw.js`) that stores the entire app (index.html plus js and css default files), which you should add files or images to as you go along. Add anything you want the user to have access to offline.

`index.html` has a single div with an id of `app`, assuming you will mount that in JavaScript, but you may delete it if not.

The only example js is the code to fire up the service worker. All other decisions are up to you. For routing, consider [navigo](https://github.com/krasimir/navigo), unless you are building in Vue or React and using their router libraries. The .htaccess file tells Apache to match all paths to the index.html file, except media files. I'm no expert on htaccess, but it has worked for me on a real project so far.

The images folder is for placing non-git-tracked images, but feel free to delete and/or change the .gitignore to fit your needs.

Speaking of which, the .gitignore file is very basic, so you may want to add to it to not accidentally track random files like .DS_Store, etc.