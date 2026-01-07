
# FAQ

---

# I’m used to using raw (pixel) values, is that wrong?

There’s nothing wrong with using raw values in Figma or code, as long as you stick to the 8px grid. This is great for exploring ideas and proving concepts.

However, when you move into the more finalized stages of design or production, your work needs to follow the Design System’s rules — especially if you’re using or updating Design System components. Space tokens are a reliable way to ensure compliance and also enable theming across different brands when needed.

Our goal has been to strike the right balance between a flexible system, which doesn’t enforce strict brand guidelines, and a more closed system that covers every situation but sacrifices simplicity.

  
![Axis - Filled](https://studio-assets.supernova.io/design-systems/161625/2448d234-b363-477d-b27e-afd676dacc5d.png)  
Axis - Filled  


The 3 solutions we studied sit at different points along a spectrum:

- **A scale system** (like t&hyphen;shirt sizes) is very simple but offers limited control across the Design System and themes. One variable can apply to many contexts, so changing it affects all those contexts.

- **A component&hyphen;based system** gives great control over spacing since each context almost has its own dedicated value. But this leads to hundreds or thousands of values, sacrificing simplicity and lightness.

- **Somewhere in between is a semantic system** that balances simplicity and control. Not every context has its own variable; instead, contexts are grouped by rules explaining how to use space. Changing a variable affects multiple contexts, but ideally only where it makes sense.

# Can I change the space of a single context?

Because the system is factored, no context is fully independent (see above). So changing spacing for just one element isn’t possible within the system’s rules. You have 2 options:

- **Create a new component **based on the one you want to edit, applying custom spacing. This counts as an “Adapt.”

- **Contact the Design System team** to discuss your needs. If your case is critical or shared by other designers, using component variables instead of semantic ones for that component might be considered. This way, you can tweak theme values for that specific context without affecting others.

# Should I use spacing tokens for Gutters or Margins?

Margins are the gaps on both sides of a page or app screen; gutters are the spaces between columns in a grid layout. Since gutters vary by Breakpoint (unlike many other spacings), they have dedicated variables.

Use these as section margins or inside components designed to span 100% of the viewport. Once all variables are set, they’ll adjust with screen size.

Learn more about [Space in pages](../space-in-pages/web.md).

# Where are size tokens?

Although size tokens use the same primitives (Numbers), they live in a different collection and are managed separately.

[Go to Size tokens](../size.md)