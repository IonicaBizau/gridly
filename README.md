[![gridly](http://i.imgur.com/kPrOESX.png)](http://ionicabizau.github.io/gridly/example/)

# gridly [![Support this project][donate-now]][paypal-donations]

The minimal (~100-170 bytes) grid system for modern browsers.

You don't need monolithic CSS frameworks for simple grid systems. ~100 bytes of CSS can save your life. :dizzy:

## Usage

In the [`dist`](/dist) directory there are three minified files:

 - `gridly-core.min.css` (105 B): just the Gridly core including same-width column support and mobile responsive support.
 - `gridly-col-widths.min.css` (92 B): the custom width columns
 - `gridly.min.css` (165 B): the previous two files' content put together

## :rocket: Available on CDN!

Gridly is available on cdnjs.com. [**Check it out**](https://cdnjs.com/libraries/gridly).

> https://cdnjs.cloudflare.com/ajax/libs/gridly/1.1.0/gridly-core.min.css
> https://cdnjs.cloudflare.com/ajax/libs/gridly/1.1.0/gridly-col-widths.min.css
> https://cdnjs.cloudflare.com/ajax/libs/gridly/1.1.0/gridly.min.css

If you do not need custom width columns, you will probably want to use only `gridly-core.min.css` in your page. If you do need the custom width columns, you have to include `gridly.min.css` instead.

## Example

Include the CSS file in your page:

```html
<link rel="stylesheet" href="gridly.min.css" type="text/css" charset="utf-8">
```

Then you can use the `.row` and `.col` classes:

```html
<div class="row">
    <div class="col">Two</div>
    <div class="col">Column</div>
</div>
```

This will create two columns having equal widths.

[![gridly](http://i.imgur.com/m4pwrnO.png)](http://ionicabizau.github.io/gridly/example/)

## Installation

Check out the [`dist`](/dist) directory to download the needed files and include them on your page.

## Documentation

The `gridly-core.min.css` file handles two classes:

 - `row`: the row containing columns
 - `col`: the column to put in the row

Because of the flexbox amazing power, the columns will have the same width (as many columns you want / row).

To extend this basic functionality, there is another file: `gridly-col-widths.min.css`. This adds the following classes:

 - `col-tenth` has `10%` width
 - `col-fifth` has `20%` width
 - `col-quarter` has `25%` width
 - `col-third` has `33.3333334%` width
 - `col-half` has `50%` width

Like specified above, the `gridly.min.css` contains both: the core and the custom widths.

## How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].

Run `npm i` to install the dependencies. Then, you can run the npm scripts using `npm run <script-name>`.

Run `npm run release` to recreate all the `dist` files.

## Where is this library used?
If you are using this library in one of your projects, add it in this list. :sparkles:

 - [showalicense.com](http://showalicense.com/)–A site to provide an easy way to show licenses and their human-readable explanations. ([source](https://github.com/IonicaBizau/showalicense.com))

## License

[MIT][license] © [Ionică Bizău][website]

[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
[donate-now]: http://i.imgur.com/6cMbHOC.png

[license]: http://showalicense.com/?fullname=Ionic%C4%83%20Biz%C4%83u%20%3Cbizauionica%40gmail.com%3E%20(http%3A%2F%2Fionicabizau.net)&year=2015#license-mit
[website]: http://ionicabizau.net
[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md