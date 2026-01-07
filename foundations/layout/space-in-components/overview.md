
# Overview

---

# Summary

Welcome’s space system aims to go beyond typical spacing systems that rely on raw values or simple semantic scales. It offers a lightweight, easy&hyphen;to&hyphen;use, shared semantic system that enables consistent control of components across different themes (brands). Inspired by [Nathan Curtis’ analysis of space](https://medium.com/eightshapes-llc/space-in-design-systems-188bcbae0d62) in digital interfaces, the system is fully platform&hyphen;agnostic and applies to Figma, web, and mobile platforms.

- Most tokens are composite, designed to serve different purposes of space, whether separating elements or surrounding them.

- A simpler, incremental scale is also available to support research and address potential edge cases.

- A simpler, incremental scale is also available to support research and address potential edge cases.

---

# The space system

## Primitives

Space shares its primitive level with other measurements in the Design System called[ Numbers](#). This means space cannot use arbitrary values; it must follow predetermined values based on the 8px grid.

## Parameters

The spacing system uses these parameters:

- **Responsiveness: **How the variable behaves across breakpoints. It can be either static — for standard, regularly sized and spaced elements that don’t change — or dynamic, mainly used for large components that need more space on Desktop but cannot keep that space on mobile (like the Billboard component).

- **Role: **The purpose of the space in context. Possible roles include:

- **Level: **The hierarchy level within the token family, ranging from none (only for zero value), min, 2xs, xs, sm, md, lg, xl, 2xl, and, if needed, 3xl, 4xl, etc., up to max.

Space can also be negative. Tokens with a neg prefix express negative spacing — for example, **neg&hyphen;3xl **with a value of &hyphen;32px, used in Highlight.

- **Responsiveness: **How the variable behaves across breakpoints. It can be either static—for standard, regularly sized and spaced elements that don’t change—or dynamic, mainly used for large components that need more space on Desktop but cannot keep that space on mobile (like the Billboard component).

- **Level: **The hierarchy level within the token family, ranging from none (only for zero value), min, 2xs, xs, sm, md, lg, xl, 2xl, and, if needed, 3xl, 4xl, etc., up to max.
[Provided bullet points for clarity; explained each parameter clearly and succinctly.]

> Some extra info:  
> Space can also be negative. Tokens with a neg prefix express negative spacing—for example, `neg&hyphen;3xl `with a value of &hyphen;32px, used in Highlight.

## Composite tokens

Some of Welcome’s space tokens are composite tokens, in the sense that one individual semantic token is a group of several primitive tokens. This applies to all tokens describing space around elements (inset, insetSquish, and insetStretch).

In CSS, space around elements is controlled by either padding or margin. Our tokens can apply to both, which is why we don’t differentiate between them. **The CSS padding property can be specified with one to four values:**

- 1 value applies the same padding to all 4 sides.

- 2 values apply padding to top and bottom, then left and right.

- 3 values apply padding to top, right and then left and bottom.

- 4 values apply padding clockwise to top, right, bottom, and left.

Composite tokens use this convention, allowing a single token to hold up to 4 sub&hyphen;values for flexible spacing.

```json  
        "insetSquish": {
          "2xs-h": {
            "$type": "spacing",
            "$value": "{wel.web.bSem.spacingStatic.insetSquish.2xs-h}",
            "$description": "minimum horizontal padding."
          },
          "2xs-v": {
            "$type": "spacing",
            "$value": "{wel.web.bSem.spacingStatic.insetSquish.2xs-v}",
            "$description": "Minimum vertical padding."
          },
      },  
```

With composite tokens like these, the following 2 instructions will produce the same result.

```css  
padding: 4px;
margin: 2px 4px;  
```

And

```css  
padding: inset-xs;
margin: insetSquish-xs-h;  
```

Since flexibility is essential, you can mix different token types to handle unusual situations or quickly prototype designs.

```css  
padding: inset-sm;
margin: space-none space-sm space-md space-none;  
```

## Responsive

In large components, spacing may change depending on the viewport size. To support this, dynamic space tokens have values defined for each Breakpoint, ranging from `mobile` to `desktop medium`.

For most tokens, values remain the same across all Breakpoints (these are static tokens). However, in some cases, spacing varies significantly between Breakpoints. For example, an inset of 64px on the `desktop medium` Breakpoint might correspond to an inset of 16px on `mobile`.

> Some extra info:  
> When using these tokens, be sure to test how your component behaves at all Breakpoints!

- **stack: **space between vertically stacked elements.

- **inline: **space between horizontally aligned elements.

- **inset: **equal space around an element.

- **insetStretch: **space around an element with larger vertical space than lateral space, making content look horizontally stretched.

- **insetSquish: **space around an element with larger lateral space than vertical space, making content look horizontally squished.

- **pinchHorizontal: **space applied only on the right and/or left of an element.

- **pinchVertical: **space applied only on the top and/or bottom of an element.