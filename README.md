# Modular CSS

In writing modular CSS we want to apply the object oriented concepts of abstraction, encapsulation, inheritence and polymorphism to CSS. 

## Abstraction

*Only the possible states and behaviours of the abstracted object are accessible, the internal implementation of the object remains hidden. By abstracting the internal implementation of the object, we make the object’s purpose easier to understand.*

Abstraction in CSS can be implemented in different ways, naming conventions for classes and ID's should decribe the role of the module within the site.

CSS properties can be abstracted as CSS variables http://caniuse.com/#feat=css-variables, there is a W3C specification for variables. CSS properties can also be abstracted using CSS preprocessors. 

## Encapsulation

*The object is structured to be self-contained, everything the object needs is available internally. The internal state of the object is not directly accessible externally except through the abstraction layer.*

CSS encapsulation can be difficult as CSS properties cascade through the style sheet and weak encapsulation is necessary to benefit from this.

As with abstraction, the selector naming convention describing the role of the module should be sufficiently unique to encapsulate the module.   

Scoped styling is a W3C specification that specifically supports encapsulation http://caniuse.com/#feat=style-scoped

## Inheritence

*Through inheritance, one object can inherit the characteristics of another object, this allows an existing object to be extended and similar objects to share properties and behaviours.*

## Polymorphism

*Different objects can respond to the same name in different ways, with the response specific to the object.*