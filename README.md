tenzen-ionic-rangeslider
===================
_Current version: tz-0.0.1

Tenzen's Ionic RangeSlider is a directive that creates an interactive slider that allows a user to change model values with Ionic's look & feel

#### Requirements

- Ionic (v1.0.0-rc.1+)
- jQuery (v1.7+)

Installation
------------

Download the files from Github or use Bower:

    $ bower install tenzen-ionic-rangeslider

Add the JS and CSS to your page:

    <script src="bower_components/tenzen-ionic-rangeslider/angular.rangeSlider.js"></script>
    <link rel="stylesheet" href="bower_components/tenzen-ionic-rangeslider/angular.rangeSlider.css">

Add the `tenzen-ionic-rangeSlider` module as a dependency for your app: `angular.module('myApp', ['tenzen-ionic-rangeSlider']);`

Bootstrap is not required.

If you use SCSS & Compass you can include the source SCSS directly into your project CSS if you add `bower_components` to your include path:

    @import "tenzen-ionic-rangeslider/scss/rangeSlider"; // requires Compass

Example
------------------

### Using model properties

The following properties are present in the scope:

    $scope.range = {
        min : 0,
        max : 100,
        minSelected : 0,
        maxSelected : 100
    }
    
So we can include the directive in the HTML like this:

    <div class="item range ngrs-range">
        <i class="icon ngrs-range-value ngrs-range-min-value">R$ {{range.minSelected}}</i>
        <div tz-range-slider min="range.min" max="range.max" model-min="range.minSelected" model-max="range.maxSelected"></div>
        <i class="icon ngrs-range-value ngrs-range-max-value">R$ {{range.maxSelected}}</i>
    </div>

Credits
-------

This was originally forked from [Daniel Crisp's](https://github.com/danielcrisp) angular-rangeslider:
https://github.com/danielcrisp/angular-rangeslider

Licence
-------

This code is released under the [MIT Licence](http://opensource.org/licenses/MIT)

Copyright (c) 2013 LUA.NET

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