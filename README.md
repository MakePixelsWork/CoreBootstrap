THIS REPOSITORY IS UNDER DEVELOPMENT AND **NOT** COMPLETE!
<br>
<br>
# CoreBootstrap

A few years ago, I build CoreBootstrap for my own website projects. I needed a quick and easy method to up- or even downgrade between the different versions of Twitter Bootstrap, without having to constantly make changes in some command-line prompt.

As a designer, I've always disliked the flat and often unneeded over-complicated command-line messages. I want to use a simple and visual pleasing interface. I previously used a combination of 2+ software packages to compile (WinLess), reload (LiveReload) and minify or even uglify code. These days I just use one compiler that does it all: PrePros, available at https://prepros.io/

## Clean frameworks
CoreBootstrap consists of clean downloads of almost all LESS and Sass frameworks of Twitter Bootstrap. Since a lot of my projects include commonly used mixin libraries, I decided to include them too. These are currently FontAwesome and LessHat.

You load the preferred versions of each source, add your own variables, code addition files... and compile your file(s) to a public folder to read in your final coded website.

Its happened to me twice that I needed to switch to an older version of Twitter Bootstrap, to make things work. The only thing I needed to do in my own CoreBootstrap, was to switch a single number, ie 3.3.5 to 3.3.4, recompile the code and voila, finished!

## My First GitHub Repository
I'm new to GitHub. I'm learning. I've decided to release my CoreBootstrap to other developers. Feel free to create additional code, expand on it, whatever. In the process I'm sure I will learn how GitHub works.

Feel free to drop me a message. I'm interested what you think of CoreBootstrap

## MIT Licence
I'm also new to licensing. Since Twitter Bootstrap itself is released under an MIT License, I've released my CoreBootstrap under the same, all in good faith. There is no copyright infringement intended.

## Current Supported Framework Versions
- Bootstrap
  - Less: 3.3.1 / 3.3.2 / 3.3.4 / 3.3.5 / 3.3.6 / 3.3.7 / 3.4.0 / 3.4.1
  - Sass: 4.0.0 / 4.1.0 / 4.1.1 / 4.1.2 / 4.1.3 / 4.2.1 / 4.3.0 / 4.3.1
- FontAwesome
  - Less: 4.2.0 / 4.3.0 / 4.4.0 / 4.5.0 / 4.6.1 / 4.6.3 / 4.7.0 / 5.0.4 / 5.0.X * / 5.1.0 / 5.1.1 / 5.2.0 / 5.3.0 / 5.3.1
  - Sass: 4.7.0 / 5.0.4 / 5.0.X * / 5.1.0 / 5.1.1 / 5.2.0 / 5.3.0 / 5.3.1
- LessHat
  - Less: 3.0.2
  - Sass: 4.1.0 **

\*)  Increments too fast, updates postponed<br>
\*\*) Not yet installed, to be decided

## How To 'Version' within the CoreBootstrap code
### (Step 1 and 2 are only needed to install a newer version)
1. Copy new DIST files to versioned PUBLIC folder (x-x-x) in:
   * /template/public/fonts/font-awesome/x-x-x/
   * /template/public/fonts/glyphicons/x-x-x/
   * /template/public/js/bootstrap/x-x-x/
2. Copy new LESS or SASS files to versioned SRC folder (x-x-x) in:
   * /template/src/**less|sass**/bootstrap/x-x-x/
   * /template/src/**less|sass**/font-awesome/x-x-x/
   * /template/src/**less|sass**/lesshat/x-x-x/
3. Update CORE TEMPLATE with:
   * Versioned 'Basic template' source code *...copied from Bootstrap website, within \<head\>*
   * Latest CDN JAVASCRIPT *...copied from Bootstrap website, at end \</body\>*
   * If applicable, versioned folder (x-x-x) for bootstrap(.min).js *...after jQuery, at end \</body\>*
4. Update /TEMPLATE/SRC/**LESS|SASS**/STYLES-LESS|SASS.EXT with:
   * Your preferred framework versions
   * Your own hierarchical positioned file(s)
5. If applicable, update /TEMPLATE/SRC/**LESS|SASS**/VARIABLES.EXT with:
   * Updated framework variables
   * Your own variables

## How To Compile
- Use a compiler, ie PrePros, available at https://prepros.io/
- Only compile /TEMPLATE/SRC/**LESS|SASS**/STYLES-**LESS|SASS**.EXT to /TEMPLATE/PUBLIC/CSS/STYLES-**LESS|SASS**.CSS

## Download ZIP
I host a downloadable ZIPPED version of the entire project on my own online test environment. This includes almost the same explanation as above. Which is also within the ZIP.<br>
\> http://www.testingoursite.com/bootstrap/ 

With best regards,

Vic van der Put
