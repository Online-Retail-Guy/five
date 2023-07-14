
<img width="125" src="https://onlineretailguy.neto.com.au/assets/images/five-logo.png">

Five started its life more or less as a direct port  of the [Skeletal](https://github.com/NetoECommerce/Skeletal) development theme for [Neto by Maropost](https://www.netohq.com/) which is the base theme framework that contains all of platform's front-end features. 

Five updates the Bootstrap framework to version 5 and since the initial port has morphed into its own development theme with different goals and ideas from the origional Skeletal theme. 

**Special note:** on browser compatibility, Bootstrap 5 only supports the latest two versions of the following Chrome, Firefox, Safari, Edge, Internet Explorer 11 (with some limitations), Opera, it may work on older browsers however you may have rendering issues using this theme in your webstore.

Please do not report issues with this theme without first checking you are using an up to date browser.

## Table of content

- [Installation](#installation)
- [Documentation](#documentation)
- [Testing](#testing)
- [Contribute](#contribute)
- [Support](#support)
- [Maintained](#maintained)

## Installation

**Direct install**

To install the latest version of Five directly from this repository you simply need to upload the `src` directory from this repository into the `httpdocs/assets/themes` directory on your Neto by Maropost website. You should also rename this new `src` directory to whatever you would like your custom theme to be named. You will want to run `npm run build` first so you have the compiled css. 

For the above, you will need SFTP access to your Neto by Maropost website, which you can request [here](https://forms.neto.com.au/design/requestftp.html).

**New theme**

For creating a new Maropost Commerce Cloud theme, you will want to use the [Theme Starter Kit](https://www.npmjs.com/package/ntheme).

## Documentation

Documentation for designers and developers can be found [here](https://developers.maropost.com/documentation/web-designers/getting-started).

As Five is built almost entirely upon Bootstrap 5, the [Bootstrap documentation](https://getbootstrap.com/docs/5.0/getting-started/introduction/) is perhaps the most valuable source of documentation for a web designer who isn't looking to build complex functionality.

## Compiling .scss files

Five uses [SASS](https://sass-lang.com/) to build its CSS. Our `.scss` files are compiled into `app.css`, avoid modifying `app.css`. Otherwise, if for whatever reason you eventually do need to re-compile the `.scss` files, any changes to `app.css` would be lost. 

You are best to develop your own `.scss` file and adding it to the imports in `src/scss/app.scss`, which needs to be compiled to `src/css/app.css` using Gulp.

If you are compiling `.scss` files for the purpose of contributing to Skeletal, follow these steps:

_Note that steps 1 and 2 only need to be completed once per system, so no need to repeat them again._

1. Install [node.js](https://nodejs.org/),
2. CD into your local folder of Five and run the `npm ci` command to install all relevant dependencies,
3. Run either of these two commands:
    - `npm run build` - this will compile your `.scss` files.
    - `npm run watch` - this will watch your `.scss` files and compile them as they change.

## Testing

We have a simple testing guide located [here](/testing.md).

## Contributing

Contributing to Five is open and welcome, please read the [contribution guidelines here](/CONTRIBUTING.md).

## Origional Creators

Origional Skeletal theme developed by [Maropost](https://www.netohq.com/).

## Maintained

Five is maintained by [Online Retail Guy](https://www.onlineretailguy.com.au/) as a labour of love for the Neto Community. Installation and implementation support is available for $300 per hour.
