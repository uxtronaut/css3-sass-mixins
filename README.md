# Some CSS3 Mixins

Here's some CSS3 Mixins I use in a lot of projects.

Included:

* `@mixin animation ($animation_name, $duration: 1s, $delay: 0, $iterations: 1, $timing: linear)`
```sass
.floating
  +animation(floating, 12s)
```
* `@mixin keyframes ($animation_name)`
```sass
+keyframes(floating)
  from
    +transform(translate(0, 0) rotate(-50deg) scale(0.95))
  50%
    +transform(translate(0, 0.66rem) rotate(-40deg) scale(1.05))
  to
    +transform(translate(0, 0) rotate(-50deg) scale(0.95))
```
* `@mixin transform($params)`
```sass
#some-element
  +transform(translate(0, 0) rotate(-50deg) scale(0.95))
```
* `@mixin transition($params)`
```sass
#some-element
  +transition(width 2s)
```

## License

(The MIT License)

Copyright (c) 2014 Zach Payne

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
