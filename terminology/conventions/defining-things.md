
# Defining things

---

Because design systems are multi&hyphen;faceted, they need a single language, independent from any of the multiple platforms covered. Below is an attempt at such a language to name all the things found in Welcome.

> Be warned:  
> Bear in mind that the following is an attempt and a goal, and by no means a reality in the current implementations of Welcome.

# Token

A token (or design token) is an atomic (there is no smaller scale) object representing a scalable design decision, unique and platform&hyphen;agnostic. It allows the syncing of platforms with different languages (namely, design and code).

Tokens are formed of a name and a value, and can be nested — one token referencing, or aliasing another with different names. In Welcome, tokens form the Design System’s [Foundations](#).

There are three classes of tokens in Welcome. Each class is distinguished from the others thanks to a prefix:

- `prim` → primitive tokens, e.g., `wel.prim.color.stratos.2`

- `sem` → semantic tokens, e.g., `wel.sem.color.loyalty&hyphen;container&hyphen;low`

- `comp` → component tokens, e.g., `wel.comp.btn.primary.fg&hyphen;color`

  
**Figma (Web)**  
In Figma for Web, tokens are variables. They combine 2 naming systems:  
- Lowercase ([kebab case](https://developer.mozilla.org/en-US/docs/Glossary/Kebab_case)) to separate each token category.  
- Capital case ([camel case](https://developer.mozilla.org/en-US/docs/Glossary/Camel_case)) for compound words  
Example: `wel.sem.text.brandName`  
  
**vue.js**  
> Some extra info:  
> Coming soon  
  
**SwiftUI (iOS)**  
In Figma for iOS App, tokens are variables, and are written in camel case. which means we start with a lowercase letter then capitalize the first letter of second and subsequent words: `onSurfacePrimary`  
  
**Compose (Android)**  
In Figma for Android App, tokens are treated as variables and follow PascalCase conventions. This means that both the first letter of the first word and each subsequent word are capitalized. For example: `OnSurfacePrimary`  


# Component

A component is a reusable, single element with a defined purpose. Sometimes UI elements can share visual and functional features, but end up being separate components because they don't provide the same experience.

Input Text and Input Currency, for example, are both inputs that share the same functionality (input data). However, due to the formatting constraints of Input Currency (only add numbers, with an attached currency icon), they are separate components because they can't be swapped in a given context.

[How to name components](../component-naming/guidelines.md)

# Pattern

For our Patterns, we follow the definitions [used by IBM’s Design System](https://carbondesignsystem.com/patterns/overview/), Carbon:

> Patterns are best practice solutions for how a user achieves a goal. They show reusable combinations of components and templates that address common user objectives with sequences and flows.

In practice, there usually is a size and/or complexity factor to separate components from patterns. But not always — common interface paradigms can also be called patterns even though their recommended implementations are simple (e.g. Loading, Notification, Error…)

# Variant

In Welcome, a variant is a version of a component that has the same UX purpose (it affords the same experience) but can have varying aspects, structure, or sub&hyphen;elements.

> Some extra info:  
> In vue.js, variants are usually documented through separate stories on Histoire. In Figma, variants can be [Figma variants](https://help.figma.com/hc/en-us/articles/360056440594-Create-and-use-variants) (a separate, albeit similar concept) or different components altogether; in both cases, variants are grouped under the same name.

# Property

A property is a simple feature that varies, according to a set of values, on a given component. Changing the value of a property, or adding a property, doesn't change the purpose, the structure, or the overall look of the component, but can help adapt it to certain use cases.

For example, `orientation` is a recurrent property that governs the layout of a component, but doesn't change its structure or elements. It usually has two values: `horizontal` and `vertical`.

> Some extra info:  
> On Figma, a property is a [similar concept](https://help.figma.com/hc/en-us/articles/5579474826519-Explore-component-properties) with different types (variant property, component property). In most cases, semantic properties are Figma properties, but for simplicity reasons, there are cases where a property value is made into a separate Figma component.

[How to name properties](../property-naming.md)