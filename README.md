# Sigrid

A **si**mple **grid** system, written in [Sass](http://sass-lang.com/ "Syntactically awesome stylesheets").

## Usage

### With regular classes

**Markup:**

    <div class="grid">
      <div class="row">
        <div class="unit one-half">
          ...
        </div>
        <div class="unit one-half">
          ...
        </div>
      </div>
    </div>

### With placeholder selectors

**SCSS:**

    .container {
      @extend %grid;
    }

    .header {
      @extend %row;
    }

    .banner,
    .nav {
      @extend %unit;
      @extend %one-half;
    }

**Markup:**

    <div class="container">
      <header class="header">
        <div class="banner">
          ...
        </div>
        <nav class="nav">
          ...
        </nav>
      </header>
    </div>


## License

**The MIT License (MIT)**

*Copyright (c) 2013 Ellen Gummesson*

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
