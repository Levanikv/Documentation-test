
# Overview

---

# Anatomy

  
![Anatomy](https://studio-assets.supernova.io/design-systems/161625/76072046-af35-44f3-be48-0a0eb3afd9ae.png)  
Anatomy  


1. **Top section** · Contains Media and optional Logo

1. **Image** · [Media](#) instance for visual content

1. **Logo** · Optional · [Logo Slot](#), positioned absolutely over the image

1. **Bottom section** · Contains all text content and interactive elements

1. **Badges row** · Optional · Container for up to 3 [Badge](#) instances

1. **Kicker** · Optional · label text providing context

1. **Title** · Primary heading text for the Callout

1. **USP** · Optional · Unique Selling Proposition with icon and descriptive text

1. **Key information** · Optional · Supporting information text

1. **Description** · Optional · Additional descriptive content

1. **CTA** · Optional · Call&hyphen;to&hyphen;action using [Button](#) instance

# Variants

## Background

Callout Editorial can display content in two background configurations: `no` and `yes`.

- **background=no (default): **Content section displays without a background surface, relying on the parent container's background for visual context.

- **background=yes: **Content section displays with a `surface&hyphen;container&hyphen;low` background, creating visual separation between the image and text content. The container applies rounded corners at the bottom, while the image container maintains rounded corners only at the top.

  
![Background](https://studio-assets.supernova.io/design-systems/161625/03b7c794-1760-428c-a9cb-55c43435441a.png)  
Background  


# Properties

Several properties give users control over Callout Editorial's behavior and appearance:

- **background**: Controls whether content appears with or without a background surface, using values `no` (default) or `yes`.

- **kicker**: Toggles the visibility of Kicker and allows content customization.

- **logo**: Toggles the visibility of [Logo Slot](#) on the image.

- **badge&hyphen;1**: Shows or hides the 1st Badge in the badges row.

- **badge&hyphen;2**: Shows or hides the 2nd Badge in the badges row.

- **badge&hyphen;3**: Shows or hides the 3rd Badge in the badges row.

- **usp**: Toggles the visibility of the Unique Selling Proposition with an icon and label.

- **key&hyphen;information**: Shows or hides the key information text element.

- **description**: Toggles the visibility of the description text.

- **cta**: Shows or hides Button.

# Behavior

## Size & breakpoints

Callout Editorial adjusts its internal spacing according to the background configuration. The component height adjusts automatically to accommodate the content within, following the visible elements.

### **Content spacing**

When background is enabled, horizontal padding uses the `insetStretch` Token for left and right padding.

### **Corner radius**

When background is enabled, the top container uses top&hyphen;only radius while the content container uses bottom&hyphen;only radius, creating a unified card appearance.

## Interaction

Callout Editorial serves as a preview element inviting users to access more content. Users can interact with the component through:

- **CTA button**: When enabled, users can click the Button to navigate to the linked content.

- **Badges**: Badges provide contextual information about the content, such as special offers, family&hyphen;friendly tags, or promotional labels. They are not clickable.

The component typically appears within a [Callout Container](#) that manages display modes (carousel or grid) and handles navigation between multiple Callout Editorial items.

## States

Callout Editorial itself doesn't have interactive states, but its child elements maintain their own state behaviors:

- **CTA button**: Follows the [Button](#) component state specifications including default, hover, pressed, focus, and disabled states.

- **Badges**: Follow the [Badge](#) component state behaviors according to their emphasis and function configurations.

- **Logo**: Follows the [Logo Slot](#) component specifications for display states.