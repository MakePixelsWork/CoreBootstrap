# CoreBootstrap

A few years ago, I build CoreBootstrap for my own website projects. I needed a quick and easy method to up- or even downgrade between the different versions of Twitter Bootstrap, without having to constantly make changes in some command-line prompt.

As a designer, I've always disliked the flat and often unneeded over-complicated command-line messages. I want to use a simple and visual pleasing interface. I previously used a combination of 2+ software packages to compile (WinLess), reload (LiveReload) and minify or even uglify code. These days I just use one compiler that does it all: PrePros, available at https://prepros.io/

## Pre-compiled
CoreBootstrap consists of clean downloads of almost all LESS and Sass versions of Twitter Bootstrap. Since a lot of my projects include commonly used mixin libraries, I decided to include them too. These are currently FontAwesome and LessHat.

You load the preferred versions of each, add your own variables, code addition files where needed... and compile your file(s) to a public folder.

Its happened to me twice that I needed to switch to an older version of Bootstrap, to make things work. The only thing I needed to do in my own CoreBootstrap, was to switch a single number, ie 3.3.5 to 3.3.4, recompile the code and voila!

## GitHub Repository
I'm new to GitHub. I'm learning. I've decided to release my CoreBootstrap to other developers. Feel free to create additional code, expand on it. And help me learn more about Git and GitHub.

Feel free to drop me a message. I'm interested what you think of CoreBootstrap

## MIT Licence
I'm also new to licensing. Since Twitter Bootstrap itself is released under an MIT License, I've released my CoreBootstrap under the same, all in good faith. No copyright infringement intended.

## Current Supported Versions
- Bootstrap
  - Less: 3.3.1 / 3.3.2 / 3.3.4 / 3.3.5 / 3.3.6 / 3.3.7 / 3.4.0 / 3.4.1
  - Sass: 4.0.0 / 4.1.0 / 4.1.1 / 4.1.2 / 4.1.3 / 4.2.1 / 4.3.0 / 4.3.1
- FontAwesome
  - Less: 4.2.0 / 4.3.0 / 4.4.0 / 4.5.0 / 4.6.1 / 4.6.3 / 4.7.0 / 5.0.4 / 5.0.X * / 5.1.0 / 5.1.1 / 5.2.0 / 5.3.0 / 5.3.1 / 5.4.1 to 5.10.1 *
  - Sass: 4.7.0 / 5.0.4 / 5.0.X * / 5.1.0 / 5.1.1 / 5.2.0 / 5.3.0 / 5.3.1 / 5.4.1 to 5.10.1 *
- LessHat
  - Less: 3.0.2
  - Sass: 4.1.0 **

* )  Increments too fast, updates postponed
** ) Not yet installed, to be decided

## How To Version in CoreBootstrap
1. Copy new DIST files to versioned PUBLIC folder (x-x-x) in:
   * /template/public/fonts/font-awesome/x-x-x/
   * /template/public/fonts/glyphicons/x-x-x/
   * /template/public/js/bootstrap/x-x-x/
2. Copy new LESS or SASS files to versioned SRC folder (x-x-x) in:
   * /template/src/**less|sass**/bootstrap/x-x-x/
   * /template/src/**less|sass**/font-awesome/x-x-x/
   * /template/src/**less|sass**/lesshat/x-x-x/
3. Update CORE TEMPLATE with:
   * Versioned 'Basic template' source code *...copied from Bootstrap website, within <head>*
   * Latest CDN JAVASCRIPT *...copied from Bootstrap website, at end </body>*
   * If applicable, versioned folder (x-x-x) for bootstrap(.min).js *...after jQuery, at end </body>*
4. Update /TEMPLATE/SRC/**LESS|SASS**/STYLES-LESS|SASS.EXT with:
   * Your preferred framework versions
   * Your own hierarchical positioned file(s)
5. If applicable, update /TEMPLATE/SRC/**LESS|SASS**/VARIABLES.EXT with:
   * Updated framework variables
   * Your own variables

## Download
I host a downloadable version on my online test environment. If you want to download a full version in a handy ZIP file, check out the following website: http://www.testingoursite.com/bootstrap/ 

With best regards,

Vic van der Put
