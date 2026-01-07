
# Property naming

How variants and properties are named in Welcome's implementations.

---

# Introduction

As stated in the [definitions section](./conventions/defining-things.md), variants and properties have a difference in degree, not nature. In Figma, while a component property can (usually) only be used to implement a property, a variant property can be used to implement a (semantic) property or a variant (with structural changes to the component). On Histoire, semantic variants are usually documented through different stories, but they are sometimes only the result of a change in (vue) properties values.

Below are some guidelines on how to name and organize properties (and variants), with precise instructions for each platforms.

> undefined  
> The property name has to be explicit. 
Stay as close a possible to the style naming related to your platform framework (css for web, Swift UI for iOS and Compose for Android)

# Order

Properties should be sorted by frequency of use (for instance, the Size property should come before the Appendix property, as it’s the first thing users will tweak).

Values of properties should follow frequency as well, starting with the default value. In the absence of a clear frequency, use alphabetical order.

# Properties

## Breakpoint

Always comes first in the property list (when applicable).

For AEM components, Property list in Figma may follow the AEM component Dialog Box property order. So Breakpoint may not comes first. 

> Be warned:  
> Breakpoint values are mandatory, since they power the [Templates](../get-started/designing/using-templates/overview.md).

  
**Figma (Web)**  
- ✏️ Name: *breakpoint*  
- 📙 Values:   
  
**Figma (App)**  
- ✏️ Name: *screen size*  
- 📙 Values: *iOS 375 &hyphen; iOS 834 &hyphen; iOS 1194 &hyphen; AND 360 &hyphen; AND 1440*  
  
**vue.js**  
> Some extra info:  
> Coming soon  


## Content

Use Content to describe variations in the component’s content. The content can be chosen from a list and/or via “slot” (when a dev places an empty customizable slot and designer can swap the slot with another component).

  
**Figma**  
- ✏️ Name: *content*  
- 📙 Values: *{semantic}, slot*  
  
**vue.js**  
> Some extra info:  
> Coming soon  


> Be warned:  
> Don’t use ‘swap’ as a name.

## Function

Function describes the semantic role of the component within the UI. For example: a Primary Button is the main action on the page.

  
**Figma**  
- ✏️ Name: *function*  
- 📙 Values: *primary, secondary, default, warning, danger, success, loyalty, offer, …*  
  
**vue.js**  
> Some extra info:  
> Coming soon  


## Size

  
**Figma**  
- ✏️ Name: *size*  
- 📙 Values: 2xs, *xs, sm, md, lg, xl, 2xl, max*  
  
**vue.js**  
> Some extra info:  
> Coming soon  


## State

  
**Figma**  
- ✏️ Name: *:state*  
- 📙 Values: *default, hover, pressed, active (or selected), disabled, open, focus…*  
  
**vue.js**  
In Web implementations, states aren’t properties but actual states that can be triggered via the Inspector. Sometimes, states can be demonstrated as stories (validation states for instance).  


## Emphasis

Describes the hierarchical level within a given function or variation.

  
**Figma**  
- ✏️ Name: *emphasis*  
- 📙 Values: *default, high, low*  
  
**vue.js**  
> Some extra info:  
> Coming soon  


## Variations

Values describe the variants according to their nature. Use it when the variant is neither a function, a size nor a content variant.

  
**Figma**  
- ✏️ Name: *type*  
- 📙 Values: *{description of types}*  
  
**vue.js**  
> Some extra info:  
> Coming soon  


> Be warned:  
> Variations are not states.

## Quantity

  
**Figma**  
- ✏️ Name: *&num; {name of the item}*  
- 📙 Values: *1, 2, 3, …*  
  
**vue.js**  
> Some extra info:  
> Coming soon  


## Display

  
**Figma**  
- ✏️ Name: *display*  
- 📙 Values: *inline, stack, carousel, grid*  
  
**vue.js**  
> Some extra info:  
> Coming soon  


## Alignement

  
**Figma**  
- ✏️ Name: *align*  
- 📙 Values: *flex&hyphen;start, center*  
  
**vue.js**  
> Some extra info:  
> Coming soon  


## Appendixes

Added, optional elements in a component. Avoid using names like start/end, prefix/suffix, prepend/append because they all rely on LTR reading paradigms. Use appendix if the content has multiple options (icon and image for instance). Add the position (left, right) if there are several appendixes.

  
**Figma**  
- ✏️ Name: *appendix*, or *left&hyphen;{name of the item} / right&hyphen;{name of the item}*  
- 📙 Values: *icon*, *image*, instance swap…  
  
**vue.js**  
> Some extra info:  
> Coming soon  


## Boolean

  
**Figma**  
- ✏️ Name: *{name of the object}*  
- 📙 Values: *true, false*  
> undefined  
> Only name the property by the name of the object, the toggle shows that it’s a hide/show property  
  
**vue.js**  
> Some extra info:  
> Coming soon  


## Instance swap

This is a Figma&hyphen;only property type:

- ✏️ Name: *{name of the object}*

- 📙 Values: *none, or {preferred instances}*

> undefined  
> The presence of a square icon shows that’s it an instance swap property (no need to add “choose” to the name)

## Text content

  
**Figma**  
- ✏️ Name: *{name of the object}*  
- 📙 Values: *{content}*  
> undefined  
> The presence of a text input shows that’s it a content property (no need to add “text” to the name)  
  
**vue.js**  
> Some extra info:  
> Coming soon  


## Child properties

In Figma, properties can be conditional to a parent (when an object is shown, it can be swapped or edited, or its children can be toggled in and out of view). In those cases:

- ✏️ Name: → *{name of the object}*

- 📙 Values: *…*

  
![Example](https://studio-assets.supernova.io/design-systems/161625/ca88353b-c292-4905-9956-2b8567e332de.png)  
Example, Here on the "left-icon" instance swap child property.  
  
