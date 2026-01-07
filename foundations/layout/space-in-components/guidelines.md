
# Guidelines

---

# Key differences between Static and Dynamic

  
| Column 1 | Column 2 | Column 3 |  
| --- | --- | --- |  
| Feature | Static Tokens | Dynamic Tokens |  
| Behavior | Fixed across all screen sizes | Adapts to different breakpoints |  
| Use cases (see [component board](https://www.notion.so/3fdd3553297b416d8f9854fb62b6c965?v=017fc498432845f88be48a9c8bc4ce25&source=copy_link)) | Accordion, Badge, Button, Callout, Chip, Checkbox, link, … | Billboard, Card, FAQ, Gallery, Heading, Highlight, Section, … |  
| Values | Generally smaller, precise | Larger and more variable |  
| Predictability | Highly predictable | Context&hyphen;dependent on breakpoint |  


# Picking tokens

Just as [color names](../../color/overview.md) reflect how and why colors are used, our space system defines the purpose of space in components. When choosing the right token, ask yourself these questions:

- Is the space static or dynamic (does it change with screen size)?

- Is the space applied around elements or between them?

- If it’s between elements, are they stacked vertically or arranged horizontally?

- If it’s around elements, what’s the proportion between lateral and top/bottom space?

- What is the relative size of the space within its category?

Answering these will guide you to select the appropriate token from among the 7 space categories.

  
![spacing](https://studio-assets.supernova.io/design-systems/161625/3e8fcf42-6c9c-4a09-bb30-1504652470d9.png)  
spacing  


All that’s left is to choose the right size on the scale. Remember, actual values may vary depending on the theme applied.

[Why can’t I use raw pixel values?](./faq.md)

> undefined  
> **Static or dynamic?** In most cases, you’ll use static space tokens. But if a component needs to adjust dynamically with screen width, consider using dynamic space tokens.

# Exceptions

To support specific use cases and simplify adoption of the semantic system, we also offer standard t&hyphen;shirt sizes (like `scale&hyphen;none`, `space&hyphen;xs`, `scale&hyphen;sm`, `scale&hyphen;md`, etc.) for quick designing.

On a case&hyphen;by&hyphen;case basis, component&hyphen;specific tokens may be created for these reasons:

- To maintain a context that shouldn’t change when other contexts update

- To add a second semantic layer on top of the first one

The overall goal is to use the right token type for each need: start with scale tokens to avoid worrying about complex space rules, then replace them with semantic tokens once your component is stable or moves into the Core library. Component&hyphen;specific tokens may be added as needed during the component’s lifecycle.

  
![Curve](https://studio-assets.supernova.io/design-systems/161625/cef8051a-fc23-4733-87de-8e6c4f4f104c.png)  
Curve  


# Using space in Figma

In Figma, the handy CSS shorthand for spacing isn’t available. Designers need to manually input values for Auto Layout’s gap property — whether vertical, horizontal, or both for wrapping Frames — as well as for padding on all sides.

By default, Figma groups top/bottom and left/right padding together, though you can separate them with a click. To work effectively with this, space tokens are broken down into enough values within Figma variables:

- `stack`** **and `inline`** **variables have a single sub&hyphen;value, which can be used directly in the Auto Layout gap field.

- `inset`** **has 1 value but needs to be applied uniformly to all sides of the object.

- `insetStretch`** **and `insetSquish`** **each have two values, 1 for vertical (**&hyphen;v**) and 1 for horizontal (**&hyphen;h**).

> undefined  
> We define space token names specifically for Auto Layout properties. Unfortunately, more precise scoping (separating gap from padding) isn’t available yet.