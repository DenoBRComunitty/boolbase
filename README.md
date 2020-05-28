# boolbase | https://denobr.com
Only two functions: one that returns true, one that returns false

## Why

By having only a single instance of these functions around, it's possible to do some nice optimizations. Eg. css-select uses these functions to determine whether a selector won't match any elements If that's the case, the DOM doesn't even need to be touched.
