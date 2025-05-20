# CoreBootstrap

> [!NOTE]
> Check the [changelog](CHANGELOG.md) for latest updates!

Back in 2014, I created CoreBootstrap for my own website projects. I needed a quick and easy method to up- or even downgrade between the different versions of Bootstrap, without having to constantly make changes, download newer/older versions or worse... get annoyed with the stupid CLI.

CoreBootstrap is build to work on any OS, right out of the box. Copy it to a new project, either keep or remove redundant versions, follow some of the pre-defined settings and initiate a compiler for **only 1 file**... and you are good to go!

### MIT License
Since Bootstrap itself is released under an MIT License, I've released my CoreBootstrap under the same, all in good faith. There is no copyright infringement intended.

## Current supported versions

- Bootstrap
  - Less:
    3.3.1 / 3.3.2 / 3.3.4 / 3.3.5 / 3.3.6 / 3.3.7 / 3.4.0 / 3.4.1
  - Sass:
    4.0.0 / 4.1.0 / 4.1.1 / 4.1.2 / 4.1.3 / 4.2.1 / 4.3.0 / 4.3.1 / 4.4.0 / 4.4.1 / 4.5.0 / 4.5.1 / 4.5.2 / 4.5.3 / 4.6.0 / 4.6.1 / 4.6.2 / 5.0.0 / 5.0.1 / 5.0.2 / 5.1.0 / 5.1.1 / 5.1.2 / 5.1.3 / 5.2.0 / 5.2.1 / 5.2.2 / 5.2.3 / 5.3.0 / 5.3.1 / 5.3.2 / 5.3.3 / 5.3.4 / 5.3.5 / 5.3.6
- Font Awesome
  - Less: 5.15.4 / 6.7.2
  - Sass: 5.15.4 / 6.7.2
- LessHat
  - Less: 3.0.2

## How to 'version' in LESS or SASS

The bolded **`less|sass`** in these steps define the _less_ or _sass_ folder and filename you choose to implement. The word 'ext' defines the extension of the files, if applicable. I've chosen to include this naming convention in the entire CoreBootstrap structure, but you can of course choose other file name(s) for you compiled CSS... i.e. simply 'styles.css'.

Step 1, 2 and 7 are only needed to install a newer version.

1. Copy new DIST files to versioned PUBLIC folder (x-x-x) in:
   - /template/public/fonts/font-awesome/x-x-x/
   - /template/public/fonts/glyphicons/x-x-x/
   - /template/public/js/bootstrap/x-x-x/
2. Copy new LESS or SASS files to versioned SRC folder (x-x-x) in:
   - /template/src/**`less|sass`**/bootstrap/x-x-x/
   - /template/src/**`less|sass`**/font-awesome/x-x-x/
   - /template/src/**`less|sass`**/lesshat/x-x-x/
3. Update CORE TEMPLATE with:
   - Versioned 'Basic template' source code _...copied from Bootstrap website, within \<head\>_
   - Latest JavaScript CDN _...copied from Bootstrap website, at end \</body\>_
   - If applicable, versioned folder (x-x-x) for bootstrap(.min).js _...at end \</body\>_
4. Update PATH /template/src/**`less|sass`**/styles-**`less|sass`**.ext with:
   - Your preferred framework versions
   - Your own hierarchical positioned file(s)
5. If applicable, update PATH /template/src/**`less|sass`**/variables.ext with:
   - Updated framework variables
   - Your own variables
6. Run your preferred compiler to create new compiled files
7. Update versioning in documentation files:
   - CHANGELOG.md
   - index.html
   - README.md

## How to compile

- Either use compiler software like [PrePros] or a compiler extension like [Live Sass Compiler], as recommended in the .vscode workspace folder
- Only compile<br>
/template/src/**`less|sass`**/styles-**`less|sass`**.ext<br>
to<br>
/template/public/css/styles-**`less|sass`**.css

### PrePros settings

- When active, PrePros detects file changes and recompiles on each save. If you add your own files and/or (re)structure, you'll need to update the settings within the PrePros software.
- PrePros constantly updates its settings file, so I've exluded it in the `.gitignore` file
- I've made a `prepros-backup.config` file available, in case you want to see the settings or update them in between different machines/projects.

## Setup templates

I've made starter setups available for both the 'builds' as well as 'HTML' files needed to run your CoreBootstrap enabled website. These templates make it easier to create your own versioned compiler and basic websites. Check the 'template/src/setup' folder for more info.

## Resources

Interested in the original source files? Check out the resources throught the links below.

- Bootstrap
  - GitHub > [Bootstrap](https://github.com/twbs/bootstrap) > [Releases](https://github.com/twbs/bootstrap/releases)
  - Website > [getbootstrap.com](https://getbootstrap.com/)
- Font Awesome
  - GitHub > [Font Awesome](https://github.com/FortAwesome/Font-Awesome) > [Releases](https://github.com/FortAwesome/Font-Awesome/releases)
  - Website > [fontawesome.com](https://fontawesome.com/)
- LessHat
  - GitHub > [LessHat](https://github.com/madebysource/lesshat/) > [Releases](https://github.com/madebysource/lesshat/releases)

## Addendum

<strong>I still use @import</strong> because the order of SCSS imports are critical for Bootstrap customization. You must first load custom variables, before Bootstrap's, so it uses our values instead of its own. Then you load their files, other frameworks, after which you can over-write their code in your own custom files. While those still can be partials, the newer SCSS module system (@use) enforces that all @use rules should come first, which conflicts with the classic @import-based Bootstrap workflow.

The reality: Bootstrap's SCSS is not fully compatible with the newer module system (@use/@forward) unless you fully refactor Bootstrap's source files (which I do not want to do). Mixing @use and @import is only safe if all @use rules come first... but this breaks the variable override patterns I need.

Bootstrap has not fully transitioned to @use/@forward yet, mainly for compatibility and inertia. Beta versions of v6 also use @import, so this could remain an issue. Unless they decide to rewrite it all, but I wonder how you over-write things then. To be continued. 

<strong>Bootstrap 5</strong> introduced lots of new features, which may break your old builds. These include Sass changes, a color system, grid updates, dropping code, new naming conventions... and lots of tweaks throughout the entire framework. If you start a new project, this does not concern you. If you upgrade from an older major version, then be sure to update your code where needed. A full migration guide can be found [here](https://getbootstrap.com/docs/5.0/migration/).

<strong>Font Awesome</strong> is somewhat backwards compatible, so I've decided to only include the latest maintained versions of each major release. v5.15.4 is the latest of 5, v6.7.2 is the latest of 6. Version 4 and lower are no longer supported.

<strong>LessHat</strong> has not been updated since july 2016, but is still one of the best LESS mixin libraries available. I postponed installing v4.1.0 because it became dependent on NPM and Grunt... which is weird, because their initial product had no dependencies at all. I've not used LESS for several years now and mainly focus on Sass developments, but I still want to implement this newer mixin library one day. So its on my todos list.

Good luck with creating your awesome projects!

**Victor van der Put**<br>
[@MakePixelsWork](https://github.com/MakePixelsWork)



<!-- 

GitHub alerts. The two spaces behind each title are needed, to make its header work both in GitHub as well as normal markdown!

> [!NOTE]  
> Highlights information that users should take into account, even when skimming.

> [!TIP]  
> Optional information to help a user be more successful.

> [!IMPORTANT]  
> Crucial information necessary for users to succeed.

> [!WARNING]  
> Critical content demanding immediate user attention due to potential risks.

> [!CAUTION]  
> Negative potential consequences of an action.

-->


<!-- Links -->
[Live Sass Compiler]: https://marketplace.visualstudio.com/items?itemName=glenn2223.live-sass

[PrePros]: https://prepros.io/



