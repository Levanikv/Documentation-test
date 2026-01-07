
# Usage

---

# Purpose

  
**When to use**  
Use Callout Editorial to present editorial content in an engaging, visual format that invites users to explore more.  

**For example:**  
- Use Callout Editorial to highlight a destination, experience, or editorial story with supporting imagery.  
- Consider Callout Editorial when you need to preview landing page content with a title, description, and call&hyphen;to&hyphen;action.  
- Use Callout Editorial to showcase branded content with optional logo placement and multiple badge types.  
  
**When not to use**  
Don't use Callout Editorial:  
- For product&hyphen;focused content with pricing information; consider[ Callout Product](#) instead  
- For marketing content; consider[ ](#)[Callout Marketing](#) instead.  


# Guidelines

> undefined  
> Use the Callout Editorial within a [Callout Container](#) that manages display modes (carousel or grid) and handles navigation between multiple Callout Editorial items. Don’t use it as a standalone

## Design

### Maintain consistent Callout configurations

All items within Callout Container should share consistent property configurations to create a unified visual experience.

Do  
[Do](https://studio-assets.supernova.io/design-systems/161625/8e747897-a0b8-4d60-bbd1-6e3928a47d95.png)[object Promise]

---

### Use Badges purposefully

Up to 3 Badges can be displayed to communicate different types of information, such as offers, family&hyphen;friendly features, or general labels. Each Badge serves a distinct function and should be used consistently.

Do  
[Do](https://studio-assets.supernova.io/design-systems/161625/34b1b58d-9d86-4275-a23e-068215d62dbd.png)[object Promise]

# Customization

## Callout Editorial background customization

Callout Editorial offers 2 background configurations that affect the overall visual treatment of the component.

### Available Callout background options

- **no** (default): Displays the content section without a background surface, allowing Callout to blend seamlessly with the page.

- **yes**: Applies a `surface&hyphen;container&hyphen;low` background to the bottom content section, creating visual separation and a card&hyphen;like appearance. When enabled, the image receives rounded corners only at the top, while the content section receives rounded corners at the bottom.

Do  
[Do](https://studio-assets.supernova.io/design-systems/161625/bd3df215-21f3-4e55-ba73-a75ec0ce8981.png)[object Promise]

### When to customize Callout’s backgrounds

Consider customizing Callout backgrounds when:

- You need to create a visual hierarchy between different content types within the same container.

- The content is displayed on complex page backgrounds.

### Implementation guidelines

**Maintain consistency**: All Callouts within a single container should typically share the same background configuration to maintain visual unity. Mixing different background levels can create visual noise and confuse users.
**Consider the container context**: If the Callout Container itself sits on a colored background, adjust the callout backgrounds accordingly to ensure sufficient contrast.

> Yay:  
> If you wish to further customize this component (structure, elements, tokens), it will be considered as an **Adapt**. In Figma, a local component needs to be created. Learn more about [local components](../../../get-started/designing/local-libraries/overview.md).

# Related

  
[Callout Container](#), The Callout Container is a flexible layout component that organizes and displays multiple callout items in either a carousel or grid format.  
  
[Callout Marketing](#), Callout Marketing displays visual and editorial marketing content. The component serves as a visual item within the Callout Container.  
  
[Callout Product](#), Callout Product displays visual and editorial product content related to hotels, rooms, meetings & events or restaurants. The component serves as a visual item within the Callout Container.  
  


Avoid mixing different callout styles within a single container.

Use Badges to highlight relevant attributes like offers or special features

Configure the Callout's background as you need