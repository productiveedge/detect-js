# _Detect JS with CSS_

The best technique for detecting when Javascript is disabled is to rely on the [Modernizr] (http://modernizr.com/) library, which is included by default, and will add a "no-js" class to the html element.

~~~
.module-something {
   .some-element {
      // sets some properties

      .no-js & {
         display: none; // do something special to some-element when js is disabled
      }
   }
}
~~~