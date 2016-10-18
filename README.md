#When do I need a semicolon?

OMG is this another Tabs vs Spaces kind of thing? :scream:! 

[Yes](https://github.com/twbs/bootstrap/issues/3057)

So... When do I need a semicolon?

Short Answer: Never*

Why?: Technically they should be used after statements, but this is optional because Javascript has this thing called "Automatic Semicolon Insertion" or ASI for short, which means that "...semicolons are automatically inserted into the source code in the situations in which they are needed"

And ASI is usually reliable

Long Answer: In this day and age it's basically a style choice and usually the key is the big C: Consistency

Why keep them?
>Because some tools that process Javascript code might break it when they don't find semicolons

Why not use them?
>It’s easier to remember when a semicolon is required vs when it is not

##Let's dig deeper...

Usually you need a semicolon when you're *declaring a variable*, *assigning a variable* or when *calling a function*

```javascript
var myFunction = function(myArg){console.log(myArg);};
```

You might need a semicolon if you do this

```javascript
var i = 0; i++
```

or if you do something like this

```javascript
clearMenus()
!isActive && $parent.toggleClass('open')
 ```


##Resources

1. [Semicolons in JavaScript are optional -  Mislav Marohnić ](http://mislav.net/2010/05/semicolons/)
2. [Your Guide to Semicolons in Javascript](https://www.codecademy.com/blog/78)
3. [ECMA Script ASI Specification](http://www.ecma-international.org/ecma-262/5.1/#sec-7.9)
4. [YDKJS - Types & Grammar: Error Correction](https://github.com/getify/You-Dont-Know-JS/blob/master/types%20&%20grammar/ch5.md#error-correction) 
5. [You Don't Need Semicolons](https://medium.com/@goatslacker/no-you-dont-need-semicolons-148d936b9cf2)
6. [Airbnb Style Guide](https://github.com/airbnb/javascript#semicolons)
7. [JS Standard Style Guide](http://standardjs.com/rules.html)

