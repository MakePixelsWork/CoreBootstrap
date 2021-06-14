# CoreBootstrap

A few years ago, I build CoreBootstrap for my own website projects. I needed a quick and easy method to up- or even downgrade between the different versions of Twitter Bootstrap, without having to constantly make changes in some command-line prompt.

As a designer, I've always disliked the flat and often unneeded over-complicated command-line messages. I want to use a simple and visual pleasing interface. I previously used a combination of 2+ software packages to compile (WinLess), reload (LiveReload) and minify or even uglify code. These days I just use one program that does it all: PrePros, available at https://prepros.io/

## Clean frameworks

CoreBootstrap consists of clean downloads of almost all major LESS and Sass frameworks of Twitter Bootstrap. Since a lot of my projects include commonly used mixin libraries, I decided to include them too. These are currently FontAwesome and LessHat.

You load the preferred versions of each source, add your own variables, code addition files... and compile your file(s) to a public folder to read in your final coded website.

Its happened to me twice that I needed to switch to an older version of Twitter Bootstrap, to make things work. The only thing I needed to do in my own CoreBootstrap, was to switch a single number, ie 3.3.5 to 3.3.4, compile the code and voila, finished!

## My first GitHub repository

I'm new to GitHub. I'm learning. I've decided to release my CoreBootstrap to other developers. Feel free to create additional code, expand on it, whatever. In the process I'm sure I will learn how GitHub works.

Feel free to drop me a message. I'm interested what you think of CoreBootstrap

## MIT Licence

I'm also new to licensing. Since Twitter Bootstrap itself is released under an MIT License, I've released my CoreBootstrap under the same, all in good faith. There is no copyright infringement intended.

## Current supported framework versions

- Bootstrap
  - Less: 3.3.1 / 3.3.2 / 3.3.4 / 3.3.5 / 3.3.6 / 3.3.7 / 3.4.0 / 3.4.1
  - Sass: 4.0.0 / 4.1.0 / 4.1.1 / 4.1.2 / 4.1.3 / 4.2.1 / 4.3.0 / 4.3.1 / 4.4.0 / 4.4.1 / 4.5.0 / 4.5.1 / 4.5.2 / 4.5.3 / 4.6.0 / 5.0.0
- FontAwesome \*
  - Less: 5.0.4 / 5.0.13 / 5.9.0 / 5.15.3
  - Sass: 5.0.4 / 5.0.13 / 5.9.0 / 5.15.3
- LessHat
  - Less: 3.0.2
  - Sass: 4.1.0 \*\*

> &nbsp;<br/>
> <span style="color:#4285f4;">**Warning**</span><br>
> Bootstrap 5 introduces new features, which may break your old builds. These include Sass changes, a color system, grid updates and lots of little throughout the entire framework.
> 
> If you start a new project, this does not concern you. If you upgrade from an older major version, then be sure to check and update your code where needed. A full migration guide can be found at https://getbootstrap.com/docs/5.0/migration/<br>
> &nbsp;

\*) Increments shown on their website ...including 5.0.4, because I still use it.<br>
\*\*) Not yet installed, to be decided.

## How to 'version' within the CoreBootstrap code

### (Step 1 and 2 are only needed to install a newer version)

The bolded **LESS|SASS** in these steps define the _less_ or _sass_ folder of filename you choose to implement. EXT defines the extension of the files, if applicable. I've chosen to include this naming convention in the entire CoreBootstrap structure, but you can of course choose other file name(s) for you compiled CSS... ie simply styles.css.

1. Copy new DIST files to versioned PUBLIC folder (x-x-x) in:
   - /template/public/fonts/font-awesome/x-x-x/
   - /template/public/fonts/glyphicons/x-x-x/
   - /template/public/js/bootstrap/x-x-x/
2. Copy new LESS or SASS files to versioned SRC folder (x-x-x) in:
   - /template/src/**less|sass**/bootstrap/x-x-x/
   - /template/src/**less|sass**/font-awesome/x-x-x/
   - /template/src/**less|sass**/lesshat/x-x-x/
3. Update CORE TEMPLATE with:
   - Versioned 'Basic template' source code _...copied from Bootstrap website, within \<head\>_
   - Latest CDN JAVASCRIPT _...copied from Bootstrap website, at end \</body\>_
   - If applicable, versioned folder (x-x-x) for bootstrap(.min).js _...after jQuery, at end \</body\>_
4. Update /TEMPLATE/SRC/**LESS|SASS**/STYLES-**LESS|SASS**.EXT with:
   - Your preferred framework versions
   - Your own hierarchical positioned file(s)
5. If applicable, update /TEMPLATE/SRC/**LESS|SASS**/VARIABLES.EXT with:
   - Updated framework variables
   - Your own variables

## How to compile

- Use a compiler, ie PrePros, available at https://prepros.io/
- Only compile /TEMPLATE/SRC/**LESS|SASS**/STYLES-**LESS|SASS**.EXT to /TEMPLATE/PUBLIC/CSS/STYLES-**LESS|SASS**.CSS

**PrePros settings**

- You can set PrePros to detect file changes in the other SCSS files, so it recompiles on each save. If you add your own, update the settings in the PrePros software.
- I have included my own 'prepros.config' in the root of this repo.
