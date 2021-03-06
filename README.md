Govhack 2016 Yes We Park
----



Full Featured Mobile HTML Framework For Building iOS & Android Apps

## Getting Started
* Clone/download this repo
  * Start building your App from changing Kitchen Sink, or from a clean template from `dist/` folder

## Server

Because Framework7 uses Ajax for navigation between pages you will need a server. So to make it work you should put dist folder (or Kitchen Sink) on a server. Or, as an option, you may use Gulp's server. Just run:

```
$ gulp server
```

  * Kitchen Sink will be available on `http://localhost:3000/kitchen-sink/`
  * Dist - on `http://localhost:3000/dist/`

## Kitchen Sink

Framework7' JS and CSS files in Kitchen Sink are temporary linked to `build/` to make development process easier on this stage. So to make it work you need to build Framework7 (see Build section) or to re-link JS and CSS files to `dist/` folder.

## Dist vs Build versions

On production use files (JS and CSS) only from `dist/` folder, there will be the most stable versions, `build/` folder is only for development purpose

## Build

Framework7 uses `gulp` to build a development (build) and dist versions.

First you need to have `gulp-cli` which you should install globally.

```
$ npm install --global gulp
```

Then install all dependencies, in repo's root:

```
$ npm install
```

And build development version of Framework7:
```
$ gulp build
```

The result is available in `build/` folder.

## Dist/Release

After you have made build:

```
$ gulp dist
```

Distributable version will available in `dist/` folder.

## Custom build

You can build custom version of Framework7 with only required components/modules. For example, if we need to include only Accordion, Modals and Tabs modules in addition to Framework 7 core: 

```
$ gulp custom -accordion,modals,tabs
```
After that you will find created `custom/` folder with generated JS and CSS files. Here is the list of available additional modules:

* cards
* accordion
* searchbar
* messages
* modals
* swipeout
* sortable
* smart-select
* virtual-list
* pull-to-refresh
* infinite-scroll
* scroll-toolbars
* tabs
* fast-clicks
* forms (means Ajax forms and forms storage)
* push-state
* swiper
* photo-browser
* picker
* calendar
* notifications

## Contributing

All changes should be commited to `src/` files. Framework7 uses LESS for CSS compliations, and concatenated JS files (look at gulpfile.js for concat files order)

If you want to help in Framework7 development and make it event better visit this page: http://www.idangero.us/framework7/contribute/

## Forum

If you have questions about Framework7 or want to help others you are welcome to special forum at http://www.idangero.us/framework7/forum/

## Docs

Documentation available at http://idangero.us/framework7/docs/

