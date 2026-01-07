
# Guidelines

---

# Composing rules

## Color on surfaces

Surfaces are the base layer for any page. You can apply other colors on top of them, but keep these points in mind:

- Applying one surface on top of another creates a visual distinction only if the top surface has a higher hierarchy level — for example, using `surface&hyphen;container&hyphen;mid`** **over `surface`.

- You can also achieve contrast by moving down the scale, like applying `surface&hyphen;container&hyphen;mid`** **over `surface&hyphen;container&hyphen;high`.

- All function containers (like `success&hyphen;container`) use color to create contrast. While technically you can apply any color on top, mixing functions — for instance, placing a `warning`** **on a `danger&hyphen;container`** **— may confuse users by sending mixed visual signals.

- Although you can use different levels of `surface&hyphen;container`** **for components or container backgrounds, avoid using `surface`** **except for page or section backgrounds.

Do  
[Do](https://studio-assets.supernova.io/design-systems/161625/378d9f01-c905-4bdd-9b9c-51dc436a79cc.png)[object Promise]  
Do  
[Do](https://studio-assets.supernova.io/design-systems/161625/2bd6af83-2eb7-405d-ab40-9432e5f7ac89.png)[object Promise]

## Color on color

Beyond surfaces, color pairings in the system are carefully controlled:

- You can always pair a color with its **own **counterpart. For example, use `on&hyphen;warning`** **text on a `warning`** **background.

- Avoid mixing colors from different families. For instance, do not combine `primary`** **with `accent&hyphen;container`.

- Mixing a color with its container variant is allowed, but note this only ensures sufficient contrast for non&hyphen;text elements (3:1), not for text. For example, use `primary&hyphen;container`** **for entire components placed on a `primary`** **background.

- When working with more complex color compositions, revert to the initial color. For example, on a `primary`** **background, you can place an `on&hyphen;primary`** **component with `primary`** **text inside. Such compositions should be used with care and moderation.

## Components on images

Situations often arise in which components need to sit on top of images. In such cases:

- When interactive components — like [Buttons](#) — are placed on top of an image, it’s mandatory to use a dark overlay beneath them for accessibility. Because we can’t control the image’s brightness (it might be very light or very dark), the dark overlay ensures enough contrast between the image and the component.

- For text placed directly on an image, an overlay is also necessary to keep good contrast in dark mode, where text usually appears white or light grey.

- If the components are static, such as [Badge](#) or [Logo Slot](#), you have the flexibility to keep them light or switch them to dark, whichever works best for your design.

  
![Image](https://studio-assets.supernova.io/design-systems/161625/e76324a2-edeb-4c2e-b87d-1d7c7e7cc3c2.png)  
Image  


> Be warned:  
> In rare cases, an **on&hyphen;image **variant of a component may be used instead of local dark mode within the default section mode.

# Using dark mode

Dark mode is available in the default theme and can be applied to any other theme. You can use it in two ways: globally, where the entire experience switches to dark mode, or locally, on specific sections or components.

## Global dark mode

This mode changes the whole experience — website or app — to dark mode. As users navigate, everything is displayed in dark mode. Users can choose this setting or let it follow their system preferences.

Currently, global dark mode exists only in design components, but it will be implemented in code platforms in the future.

> Be warned:  
> Currently, global dark mode exists only in design components, but it will be implemented in code platforms in the future.

## Local dark mode

Local dark mode applies dark styling to a section or component, helping create visual rhythm and boundaries on a page. This replaces what was previously called “inverse” in the old color system.

Before, we needed to create inverse color equivalents for every color and component to work on dark backgrounds. With local dark mode, those extra variations are no longer necessary.

  
![Local](https://studio-assets.supernova.io/design-systems/161625/723db2b6-4cc1-45a2-89fe-94264d7f2c30.png)  
Local  


> undefined  
> In Figma, you can create dark mode sections by switching the Mode from light to dark in the right panel, next to the “Layer” section.

When you switch a section to local dark mode, consider how it will appear in global dark mode. There are two options:

- The section “inverts” as well, showing in local light mode when the entire app is in dark mode.

- Or it remains in dark mode regardless
This behavior should be specified in your designs.

# Elevation

[Material offers](https://m3.material.io/styles/elevation/applying-elevation) a color scale for elevated content (objects that appear above the base page, along a z&hyphen;axis). Welcome’s new color system manages this concept using `surface&hyphen;container`** **tokens.

While there isn’t a formal specification yet for elevated content or shadows, here are some recommendations to guide you when creating elevated elements:

- **Level 0 **uses `surface`** **for the page background.

- **Level 1 **uses `surface&hyphen;container&hyphen;low`. Use it for purely cosmetic elevation, where the background and shadow create a visual boundary but don’t elevate the element above the base level.

- **Level 2 **uses `surface&hyphen;container&hyphen;mid`. This is ideal for elements that appear above the base page without taking full focus — overlapping it to add information, like [Popovers](#).

- **Level 3 **uses `surface&hyphen;container&hyphen;hi`, reserved for [Modals](#) or components that take focus away from the base page, such as navigation menus.

The guidelines above serve as recommendations. You can also use multiple levels of `surface&hyphen;container`** **to build a clear visual hierarchy, beyond just the technical aspects of elevation.

> undefined  
> Keep in mind that while `surface&hyphen;container`** **colors are typically white in the light theme, they shift to lighter shades of gray in dark mode. This adjustment helps maintain visibility since shadows are less visible on dark backgrounds.

`surface&hyphen;container` can be applied on top of any `surface`.

Don't create confusing feedback by mixing functions in surfaces and containers.