# SASS Set up Bootstrap

Simple starting set up of SCSS files including Bootstrap, fonts, common rules and interesting variables.

## Folder structure

```

fonts   /Merriweather.woff
        /OpenSans.woff (stack)

scss    /bootstrap  /mixins
                    /utilities
                    /vendor
                    /bootstrap.scss
        
        /_fonts.scss
        /_footer.scss
        /_front-page.scss
        /_general.scss
        /_header.scss
        /_modules.scss
        /_normalise.scss
        /_page.scss
        /_sliders.scss
        /_typography.scss
        /_variables.scss

```

## How to use

[Install SASS](https://sass-lang.com/install) if not done so already.

The SASS set up will compile all of the .scss files into one style.css file in the root of the project folder.

Copy Contents of folder into the root of your project and run the following command from the command line or Git Bash:

### Unminified version

```

sass --watch scss/_modules.scss:style.css

```

### Minified version

```

sass --watch scss/_modules.scss:style.css --style compressed

```

## Existing styles

If you are working with an existing stylesheet you can copy it into one of the .scss files or create a new one and @import it in the _modules.scss_.

The SASS set up will compile alll of the .scss files into one style.css file replacing any style.css file that was there before.