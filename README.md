# Simple Sass example

## What this is

This is a simple example for setting up Sass.

You could incorporate this into a WordPress theme, an Eleventy project, any place where you want to write [Sass](https://sass-lang.com/) and compile it to CSS.

## Instructions for setting this up

To set up this example, I:
- created an empty package.json file
- added Sass as a dependency to the package.json file
- created some Sass files
- added scripts to the package.json file for easily watching and compiling.



To create an empty package.json, run `npm init --yes` in the terminal.

After that, add sass by running `npm add sass`

After that, you can run sass in the command line by running `npx sass [INPUT_PATH]:[OUTPUT_PATH]`. For example, `npx sass src/scss/style.scss:style.css`

If you want sass to watch your Sass files and recompile whenever you make changes, add `--watch` to the command. For example, `npx sass src/scss/style.scss:style.css --watch`

Here is the documentation for Sass' command line interface:
https://sass-lang.com/documentation/cli/dart-sass

To make it easier to run the command, you can add scripts to the `package.json` file.

For example, you can set:

- the `watch:sass` script to run `npx sass src/scss/style.scss:style.css --watch` 
- the `build:sass` script to run `npx sass src/scss/style.scss:style.css`

Then you only need to run `npm run watch:sass` instead of writing out the sass command each time.