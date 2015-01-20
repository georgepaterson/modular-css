# Modular CSS

Writing modular CSS..

## Object oriented principles

In writing modular CSS we want to apply the object oriented principles of abstraction, encapsulation, inheritence and polymorphism to CSS. 

### Abstraction

*Only the possible states and behaviours of the abstracted object are accessible, the internal implementation of the object remains hidden. By abstracting the internal implementation of the object, we make the object’s purpose easier to understand.*

Selectors are the primary abstraction layer for CSS; classes and ID's should be used to change the properties of an element. Naming conventions for CSS selectors should decribe the role of the module within the site, making the element's role within the site easier to understand.

Additionally, CSS properties can be abstracted as CSS variables http://caniuse.com/#feat=css-variables, creating an internal abstraction layer during development. Although there is a W3C specification for variables, CSS properties can also be abstracted using CSS preprocessors.
 

### Encapsulation

*The object is structured to be self-contained, everything the object needs is available internally. The internal state of the object is not directly accessible except through the abstraction layer.*

The abstraction layer are the selectors, the internal state are the CSS properties of the selected element.  

CSS encapsulation can be difficult as CSS properties cascade through the style sheet and weak encapsulation is necessary to benefit from this. At times it may even be necessary to directly apply CSS properties to an element through inline styling but in general this should be avoided and styling applied through the abstraction layer. The selector naming convention describing the role of the module should be unique to encapsulate the module.   

Scoped styling is a W3C specification that specifically supports encapsulation http://caniuse.com/#feat=style-scoped allowing styles to be scoped to a specific part of the document.

### Inheritence

*Through inheritance, one object can inherit the characteristics of another object, this allows an existing object to be extended and similar objects to share properties and behaviours.*

Inheritence is a fundamental part of CSS; but the cascade must be controlled to benefit from inheritence. Using structured naming conventions an element can inherit only the CSS properties sufficient to meet the visual design. 


### Polymorphism

*Different objects can respond to the same name in different ways, with the response specific to the object.*

A CSS selector's properties can be changed based on an additional selector either on the original element, or on it's parent or sibling element.


