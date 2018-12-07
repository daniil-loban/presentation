# presentation

created on the basis of the Raveal.JS by framework (https://github.com/hakimel/reveal.js)
published at https://daniil-loban.github.io/presentation/

TRANSCRIPT:

INTRODUCTION

Welcome to Sass.
Sass is an advanced version of CSS.
As a matter of fact, any valid CSS is valid Sass.

OWERVIEW

Sass just adds features on top of CSS, it’s a kind of meta language. 
Unfortunately, at this point, no browsers support Sass files directly, so we write some Sass and then we compile or convert Sass into CSS. 

IMPORT

Sass will take the file that you want to import and combine it with the file you're importing into, so you can serve a single CSS file to the web browser.

NESTING

(a slide with CSS without nesting)
Look how much repetition there is in this file

(a slide with SCSS with nesting)
See it in Sass.
Using nesting we can easily get the combinations of selectors we need, simply by putting one block with the CSS rules into another. 
It turns out compact and clear, because we know exactly what it depends on.

VARIABLES

All variables in Sass are prefixed with a $ sign. 
Assigning a variable looks a lot like typing in a CSS property. 
Variables allow you to store some values and then substitute them in the right place in the code. 
Thus, we set the value in one place, and Sass already duplicates it on its own. 

EXTENDS

Extend clones the attributes from one class or ID and adds them to another.
Say we want to use the blue button style for the checkout button. 
All we need to do is use @extend, followed by the blue button class in the declaration of your selector.

MIX INS

Mix ins are some of the more powerful elements of Sass. 
They are analogs of functions in programming languages.
A mix in is a fragment of Sass that can easily be applied to another selector.
Mix ins can include arguments that allow you to vary your values.
To define a mix in, all you need to type is @mixin, followed by the name of the mix in and then its styling.
When you want to use the mix in, just type @include 
It’s useful to have mix ins in a separate style sheet, keeping your main style sheet cleaner.

CALCULATING A LAYOUT

In Sass, you can add, subtract, multiply and divide different sizes, getting new values.
All this is easily combined with variables, so we do not need to calculate many things on our own. 
If you mix units, Sass will try to make them work, but if they are incompatible, Sass will display an error.
For instance, you can’t multiply a px value by a em value. It just doesn’t make sense.

CONDITIONAL EXPRESSIONS

Virtually no programming language can do without the if and else statements.
In Sass, it is also possible to execute a set of commands only if the specified conditions are true.
There are lots of situations where we might want our mix ins to act smart and react to the values that we pass in.

LOOPS

(@for)

Using cycles, you can make repetitions of code fragments that differ only slightly.
The @for directive comes in two forms:
the keyword 'through' specifies the range including both the values of 'start' and 'end'.
the keyword 'to' specifies the range from 'start' value to the value before 'end' value.

(@each)

The @each directive is a trick to keep your Sass DRY (the tenet of Don’t Repeat Yourself). 
It’s a way of copying the same style for a lot of different variables.

(@while)

The @while directive takes a SassScript expression and repeatedly emits the nested block of styles until the statement evaluates to false.

FUNCTIONS

Sass offers a variety of functions.
To learn more about functions check out the Sass documentation.

