
# Maintain your library

---

# Add a new component

## Import a component

If you’ve already created components in your design files, follow these steps to move them into your local library without breaking dependencies:

1. Publish your design file as a library (see [wiki](https://help.figma.com/hc/en-us/articles/360025508373-Publish-a-library)).

1. Ensure your local library is published.

1. Cut and paste the master component from your design file into the local library (see [wiki](https://help.figma.com/hc/en-us/articles/4404848314647-Move-published-components)).

## Create from scratch

To create a local component directly in an existing file, follow these steps:

- Create a dedicated branch for each new or updated component.

- Name the branch after the component and the job to be done (for Product Designers).

- Design the component.

- Name the component according to [local naming guidelines](../../../terminology/component-naming/in-figma.md).

- Document the component thoroughly.

- [Write the changelog](./maintain-your-library.md) beside the component using the [Advanced changelog](https://www.figma.com/community/widget/1142539867133322876) widget.

- Mark the master component as “ready for dev” (</>).

- Merge the branch, adding the changelog text and title in the description.

- Publish the library.

> undefined  
> If you don’t have a local library yet, contact your Design System Manager (DSM).

# Name and organize layers.

Visit the [Terminology](../../../terminology/property-naming.md) section to learn our conventions for naming layers, variants, and properties. Following them is encouraged but not mandatory.

> Be warned:  
> The only mandatory convention is following [component naming guidelines](../../../terminology/component-naming/in-figma.md), including the correct emoji and prefix.

# Specify and document

Depending on your implementation needs, consider specifying and documenting your component by addressing:

- How it behaves at different breakpoints

- Customization options

- Possible interactions

> Some extra info:  
> Thanks to Dev Mode, it isn’t necessary to specify sizes, spacing, or properties in detail. Use the [Propstar](https://www.figma.com/community/plugin/1116018586739867857/propstar) Figma plugin to showcase allowed property combinations.

# Write a changelog

While a detailed changelog isn’t mandatory for local libraries to speed up the process, it’s good practice to include one:

- Use the [Advanced changelog](https://www.figma.com/community/widget/1142539867133322876) widget in Figma to document changes beside your component.

- Include an updated description in the branch.

- Add release date and optional summary in the publish dialog.

# Handoff to developers

> Be warned:  
> Before handing off, designers should ensure their components align with code logic and best practices (CSS or mobile OS standards).
To ease the handoff, share these resources with developers:

- [Dev Mode](https://www.figma.com/dev-mode/): For quick inspection, code suggestions, and [adding annotations](https://help.figma.com/hc/en-us/articles/20774752502935-Add-measurements-and-annotate-designs-in-Dev-Mode) directly on designs.

- [Version history](https://help.figma.com/hc/en-us/articles/360038006754-View-a-file-s-version-history): Helps check branch merges, updates, fixes, and library versions.

- **Documentation**: Offers deeper insights into behavior, motion, examples, and guidelines, hosted on Notion, Confluence, or Figma.