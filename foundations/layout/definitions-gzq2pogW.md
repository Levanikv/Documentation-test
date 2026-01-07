
# Definitions

Here is some vocabulary to help you better understand the Layout section. Keep reading to learn about space, gutters, breakpoints, and other sizing concepts.

---

**Layout **is a category that groups all variables controlling how elements are positioned and how much space they occupy on any given page. Several key concepts influence layout:

# Grid

The Grid is the foundational frame where elements are placed. It’s defined by parameters such as:

- **Columns **: the number of vertical divisions in the grid

- **Gutters **: the spaces between columns

[Learn more about Grid](./grid-and-breakpoints/breakpoints-web.md)

# Breakpoints

Breakpoints are crucial for layouts. They define screen widths at which a page’s layout adjusts to better fit the available space.

While fully customizable, Welcome’s breakpoints are fairly standard, matching common device sizes like mobile phones, tablets, and small to large monitors.

[Learn more about Breakpoints](./grid-and-breakpoints/breakpoints-web.md)

# **Space**

Space is a shorter way to say “spacing” and refers to any measure of distance — or lack of it — between elements in the user interface. It’s usually controlled by concepts like padding, margin, gap in CSS, and Auto Layout properties in Figma.

In Welcome, we handle two types of space differently, each with dedicated variables:

- **Space in pages **(or sections), mostly used with Templates. These variables manage things like the space after headings or between sections.

- **Space in components **operates one level down the atomic scale and controls spacing inside components (which can be any container, not just Welcome components). This follows a custom system.

In Welcome, we handle two types of space differently, with dedicated variables:

- [Space in pages](./space-in-pages/web.md) (or sections), mainly used with [Templates](../../get-started/designing/using-templates/overview.md). These variables control things such as the space after headings, or between sections.

- [Space in components](./space-in-components/overview.md) operates one level down the atomic scale and controls spacing inside components (which can be any container, not just Welcome components). This follows a custom system.

> Some extra info:  
> For clarity and readability, we use the word “space” instead of “spacing” throughout this documentation and in variable names, since shorter names work better.

# Size

Size controls the physical dimensions — height and width — of elements. Size variables are rare in our Design System.

- Page sizes work closely with Breakpoints to create flexible and powerful Templates.

- Certain assets, like icons, have fixed sizes that apply across the system.

- On a case&hyphen;by&hyphen;case basis, some component sizes have dedicated variables.

> Some extra info:  
> In general, component size is managed by a user&hyphen;facing property with semantic values like `sm`, `md`, and `lg`, rather than a variable.

[Learn more about Size](./size.md)

# Density

Put simply, density means “[how many things we see in a given space](https://matthewstrom.com/writing/ui-density/).” It results from all the variables and concepts we've discussed so far. While our goal is to make density a global, user&hyphen;adjustable setting, it’s currently available only in select Components as a property.