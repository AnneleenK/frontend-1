# Table of Contents

- [This or that](#this-or-that)
- [This all makes sense now](#this-all-makes-sense-now)
- [Objects](#objects)
- [Mixing up class objects](#mixing-up-class-objects)
- [Prototypes](#prototypes)
- [Behavior delegation](#behavior-delegation)
- [ES6 Class](#ES6-class)
- [Thank You](#thank-you)
- [College Notes](#college-notes)

## This or that

## Why?
```This``` allows functions to be reused against multiple _context_ objects, rather than needing a seperate version of the function for each object.  
```This``` **DOES NOT** refer to a function's lexical scope.

```This``` is not an author-time binding but a runtime binding. It is contextual based on the conditions of the function's invocation. ```This``` binding has nothing to do with where a function is declared, but has instead everything to do with the manner in which the function is called.

```This``` is actually a binding that is made when a function is invoked, and what it references is determined entirely by the call-site where the function is called.

## This all makes sense now
**Call site**: the location in code where a function is called (not where it's declared).  
**Call stack**: the stack of functions that have been called to get us to the current moment in execution.  
**Tip**: To see the call stack, go to the developer tools in the browser and set a breakpoint on the function. The tool will show you a list of functions that have been called to get to that line, which will be your call stack. Now find the second item from the top, that will show you the real call-site.  

###

## Objects

This is an h3 heading

## Mixing up class objects

This is an h1 heading

## Prototypes

This is an h2 heading

## Behavior delegation

## ES6 Class

This is an h3 heading

## Thank You

## College Notes

### This
- Runtime binding. 
- Verwijst naar de context waar je op het moment in zit, niet naar de scope.

``` javascript
var clowns = new Array() // array literal (met new maak je een object aan)
var clown = {
  name: 'Pipo', //name: key - pipo: value
  shoeSize: 80,
  laugh: function(){
    console.log('Ik heet ' + clown.name + ' hahahaha')
    console.log('Ik heet ' + this.name + ' hahahaha')
  }
} // object literal
```

Een object kan **properties** of **methods** hebben.
Properties: een clown heeft een naam, een schoen een maat. (key/value pairs)
Methods: een clown kan lachen/huilen (acties die een clown kan uitvoeren)

**Dot notation:** methods en properties aanroepen. Zoals ```clown.name``` of ```this.name```.  
**This:** This wordt in de scope van de functie automatisch gegenereerd en het verwijst naar het object waar je op dat moment in zit, oftewel de context.

### Constructor functie
Alleen *constructor* functies beginnen met een hoofdletter.
Soort blauwdruk waar je aan de hand daarvan objecten kan maken.



