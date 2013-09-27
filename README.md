# Sigrid

A **si**mple **grid** system, written in [Sass](http://sass-lang.com/).

## Requirements

You need to use `box-sizing: border-box;`.

## Configuation

### Classes

#### `$use-classes`

If this is set to `true`, classes will be used in the generated code instead of placeholder selectors.

## Usage

### With regular classes

**Markup:**

~~~ html
<div class="grid">
  <div class="grid__item  one-half">
    ...
  </div>
  <div class="grid__item  one-half">
    ...
  </div>
</div>
~~~

### With placeholder selectors

**SCSS:**

~~~ scss 
.header {
  @extend %grid;
}

.banner,
.nav {
  @extend %grid__item;
  @extend %one-half;
}
~~~

**Markup:**

~~~ html
<header class="header">
  <div class="banner">
    ...
  </div>
  <nav class="nav">
    ...
  </nav>
</header>
~~~

## License

**The MIT License (MIT)**

*Copyright (c) 2013 Ellen Gummesson*

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
