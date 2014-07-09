# CSS CLEARS

  Mobile-first classes for css-clears.
  Set the desired css-clears on any element for any breakpoint.
  Base class names are namespaced across three breakpoints:

*  -ns = not-small (covers everything larger than mobile)
*  -m  = medium
*  -l  = large

## Install
```
npm install --save-dev css-clears
```
or download the css on github and include in your project.

## File Size


## The Code
```
.cn { clear: none; }
.cl { clear: left; }
.cr { clear: right; }
.cb { clear: both; }

/* Nicolas Gallaghers Clearfix solution
   Ref: http://nicolasgallagher.com/micro-clearfix-hack/ */

.cf:before,
.cf:after { content: " "; display: table; }
.cf:after { clear: both; }
.cf {       *zoom: 1; }

@include break(not-small) {
  .cn-ns { clear: none; }
  .cl-ns { clear: left; }
  .cr-ns { clear: right; }
  .cb-ns { clear: both; }
  .cf-ns:before,
  .cf-ns:after { content: " "; display: table; }
  .cf-ns:after { clear: both; }
  .cf-ns {       *zoom: 1; }
}

@include break(medium) {
  .cn-m { clear: none; }
  .cl-m { clear: left; }
  .cr-m { clear: right; }
  .cb-m { clear: both; }
  .cf-m:before,
  .cf-m:after { content: " "; display: table; }
  .cf-m:after { clear: both; }
  .cf-m {       *zoom: 1; }
}

@include break(large) {
  .cn-l { clear: none; }
  .cl-l { clear: left; }
  .cr-l { clear: right; }
  .cb-l { clear: both; }
  .cf-l:before,
  .cf-l:after { content: " "; display: table; }
  .cf-l:after { clear: both; }
  .cf-l {       *zoom: 1; }
}

```

## Author

[http://mrmrs.cc](http://mrmrs.cc - Entire internet gateway to all things mrmrs)
[http://mrmrs.io](http://mrmrs.io - Open source projects)

## License

The MIT License (MIT)

Copyright (c) 2014 @mrmrs

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

