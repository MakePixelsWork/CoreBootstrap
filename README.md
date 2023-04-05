# CoreBootstrap

Back in 2014, I created CoreBootstrap for my own website projects. I needed a quick and easy method to up- or even downgrade between the different versions of Bootstrap, without having to constantly make changes, download newer/older versions or worse... get annoyed with the stupid CLI.

CoreBootstrap is build to work on any OS, right out of the box. Copy it to a new project, remove redundant versions, follow some of the pre-defined settings, or initiate a compiler for only 1 file... and you are good to go!

### MIT Licence
Since Bootstrap itself is released under an MIT License, I've released my CoreBootstrap under the same, all in good faith. There is no copyright infringement intended.

## Current supported versions

- Bootstrap
  - Less:
    3.3.1 / 3.3.2 / 3.3.4 / 3.3.5 / 3.3.6 / 3.3.7 / 3.4.0 / 3.4.1
  - Sass:
    4.0.0 / 4.1.0 / 4.1.1 / 4.1.2 / 4.1.3 / 4.2.1 / 4.3.0 / 4.3.1 / 4.4.0 / 4.4.1 / 4.5.0 / 4.5.1 / 4.5.2 / 4.5.3 / 4.6.0 / 4.6.1 / 4.6.2 / 5.0.0 / 5.0.1 / 5.0.2 / 5.1.0 / 5.1.1 / 5.1.2 / 5.1.3
- Font Awesome
  - Less: 4.7.0 / 5.15.4 / 6.2.1
  - Sass: 4.7.0 / 5.15.4 / 6.2.1
- LessHat
  - Less: 3.0.2

## How to 'version' in LESS or SASS

The bolded **LESS|SASS** in these steps define the _less_ or _sass_ folder or filename you choose to implement. The word 'ext' defines the extension of the files, if applicable. I've chosen to include this naming convention in the entire CoreBootstrap structure, but you can of course choose other file name(s) for you compiled CSS... i.e. simply 'styles.css'.

Step 1 and 2 are only needed to install a newer version.

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
   - Latest JavaScript CDN _...copied from Bootstrap website, at end \</body\>_
   - If applicable, versioned folder (x-x-x) for bootstrap(.min).js _...at end \</body\>_
4. Update PATH /template/src/**less|sass**/styles-**less|sass**.ext with:
   - Your preferred framework versions
   - Your own hierarchical positioned file(s)
5. If applicable, update PATH /template/src/**less|sass**/variables.ext with:
   - Updated framework variables
   - Your own variables

## How to compile

- Use a compiler, ie PrePros, available at https://prepros.io/
- Only compile<br>
/template/src/**less|sass**/styles-**less|sass**.ext<br>
to<br>
/template/public/css/styles-**less|sass**.css

### PrePros settings

- When active, PrePros detects file changes and recompiles on each save. If you add your own files and/or (re)structure, you'll need to update the settings within the PrePros software.
- PrePros constantly updates its settings file, so I've exluded it in the .gitignore file
- I've made a 'prepros-backup.config' file available, in case you want to see the settings or update them in between different machines/projects.
- Check the PrePros website for more info.

## Resources

Interested in the original source files? Check out the resources throught the links below.

- Bootstrap
  - GitHub > <a href="https://github.com/twbs/bootstrap">Bootstrap</a> > <a href="https://github.com/twbs/bootstrap/releases">Releases</a>
  - Website > <a href="https://getbootstrap.com/">getbootstrap.com</a>
- Font Awesome
  - GitHub > <a href="https://github.com/FortAwesome/Font-Awesome">Font Awesome</a> > <a href="https://github.com/FortAwesome/Font-Awesome/releases">Releases</a>
  - Website > <a href="https://fontawesome.com/">fontawesome.com</a>
- LessHat
  - GitHub > <a href="https://github.com/madebysource/lesshat/">LessHat</a> > <a href="https://github.com/madebysource/lesshat/releases">Releases</a>

## Addendum

<strong>Bootstrap 5</strong> introduced lots of new features, which may break your old builds. These include Sass changes, a color system, grid updates, dropping code, new naming conventions... and lots of tweaks throughout the entire framework. If you start a new project, this does not concern you. If you upgrade from an older major version, then be sure to update your code where needed. A full migration guide can be found <a href="https://getbootstrap.com/docs/5.0/migration/">here</a>.

<strong>Bootstrap 5.2.0 and up</strong> introduce some new stuff which I need to test, before I can upgrade my own CoreBootstrap. It may involve a different method of compiling the main Sass file, which may not be backwards compatible. I'm now thinking about writing custom compiler files, per version. To be decided.

<strong>Font Awesome</strong> is fully backwards compatible, so I've decided to only include the latest version of each major release. 4.7.0 is the latest of v4, 5.15.4 the latest of v5, etc etc

<strong>LessHat</strong> has not been updated since july 2019, but is still one of the best LESS mixin libraries available. I postponed installing v4.1.0 because it became dependent on NPM and Grunt... which is weird, because their initial product had no dependencies at all. I've not used LESS for several years now and mainly focus on Sass developments, but I still want to implement this newer mixin library one day. So its on my todos list ;).

Good luck with creating your awesome projects!

<strong>Victor van der Put</strong><br>
@MakePixelsWork

