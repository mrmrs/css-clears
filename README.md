# css-clears 1.0.6

Css module of single purpose classes for clears

#### Stats

343 | 32 | 32
---|---|---
bytes | selectors | declarations

## Installation

#### With [npm](https://npmjs.com)

```
npm install --save-dev css-clears
```

Learn more about using css installed with npm:
* https://webpack.github.io/docs/stylesheets.html
* https://github.com/defunctzombie/npm-css

#### With Git

http:
```
git clone https://github.com/tachyons-css/css-clears
```

ssh:
```
git clone git@github.com:tachyons-css/css-clears.git
```

## Usage

#### Using with [Postcss](https://github.com/postcss/postcss)

Import the css module

```css
@import "css-clears";
```

Then process the css using the [`tachyons-cli`](https://github.com/tachyons-css/tachyons-cli)

```sh
$ npm i -g tachyons-cli
$ tachyons path/to/css-file.css > dist/t.css
```

#### Using the css

##### CDN
The easiest and most simple way to use the css is to use the cdn hosted version. Include it in the head of your html with:

```
<link rel="stylesheet" href="http://unpkg.com/css-clears@1.0.6/css/css-clears.min.css" />
```

##### Locally
The built css is located in the `css` directory. It contains an unminified and minified version.
You can either cut and paste that css or link to it directly in your html.

```html
<link rel="stylesheet" href="path/to/module/css/css-clears">
```

#### Development

The source css files can be found in the `src` directory.
Running `$ npm start` will process the source css and place the built css in the `css` directory.

## The css

```css
/*
   CLEARS
*/
.cn { clear: none; }
.cl { clear: left; }
.cr { clear: right; }
.cb { clear: both; }
/* Nicolas Gallaghers Clearfix solution
   Ref: http://nicolasgallagher.com/micro-clearfix-hack/ */
.cf:before, .cf:after { content: " "; display: table; }
.cf:after { clear: both; }
.cf { *zoom: 1; }
@media screen and (min-width: 48em) {
 .cn-ns { clear: none; }
 .cl-ns { clear: left; }
 .cr-ns { clear: right; }
 .cb-ns { clear: both; }
 .cf-ns:before, .cf-ns:after { content: " "; display: table; }
 .cf-ns:after { clear: both; }
 .cf-ns { zoom: 1; }
}
@media screen and (min-width:48em) and (max-width: 64em) {
 .cn-m { clear: none; }
 .cl-m { clear: left; }
 .cr-m { clear: right; }
 .cb-m { clear: both; }
 .cf-m:before, .cf-m:after { content: " "; display: table; }
 .cf-m:after { clear: both; }
 .cf-m { zoom: 1; }
}
@media screen and (min-width: 64em) {
 .cn-l { clear: none; }
 .cl-l { clear: left; }
 .cr-l { clear: right; }
 .cb-l { clear: both; }
 .cf-l:before, .cf-l:after { content: " "; display: table; }
 .cf-l:after { clear: both; }
 .cf-l { zoom: 1; }
}
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## Authors

* [mrmrs](http://mrmrs.io)
* [johno](http://johnotander.com)

## License

ISC

