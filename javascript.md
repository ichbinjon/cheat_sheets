# Javascript cheat sheet

## function declaration vs function expression
Function declarations are hoisted up to their scope whereas function expressions remain where they are.

## Functions are hoisted first
Function declarations and variable declarations are both hoisted but functions are on top. (Assignment is never hoisted!)

## Closures
[Closure](https://github.com/getify/You-Dont-Know-JS/blob/master/scope%20%26%20closures/ch5.md) is when a function is able to remember and access its lexical scope even when that function is executing outside its lexical scope.

if a nested function `bar` inside `foo` holds a reference to the scope of `foo`, this reference is called the closure. `bar` has a closure over `foo`. Closure lets the function continue to access the lexical scope it was defined in at author-time. Very useful to know when passing around functions as args.

## Merging two lists of objects based on property
```javascript
const mergeArrayOfObjects = (original, newdata, selector = 'key') => {
        newdata.forEach(dat => {
          const foundIndex = original.findIndex(ori => ori[selector] === dat[selector]);
          if (foundIndex >= 0) original.splice(foundIndex, 1, dat);
          else original.push(dat);
        });

        return original;
      };

```
