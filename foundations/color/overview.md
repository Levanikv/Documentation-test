
# Overview

---

# Summary

Color is the most complex set of tokens in Welcome because it serves multiple brands, contexts, and users. Introduced in 2024, the new color system draws inspiration from [Google’s Material colors](https://m3.material.io/styles/color/roles) and supports both multi&hyphen;brand theming and dark mode.

- **Primitive colors** can vary from one brand to another. You can find them in the [Brand Primitives](https://www.figma.com/files/678338461349688440/project/275253087/Brand-Primitives?fuid=1484589493834517909) repository (one file per brand).

- **Semantic colors** are built on top of primitives and shared across all brands in the [🌈 [Platform name] Appearances ](https://www.figma.com/design/HXpmNTzVqJhYs57bt2UJ11/%F0%9F%8C%88-Web-Appearances?m=auto&node-id=2408-2273&t=ZwaE3Eh48P6EHmgA-1)files (one file per platform).

- **Component colors** reference semantic colors for specific UI elements.

The naming system used for Semantics is designed to simplify the use of color: the role, importance, and function of each color can be known directly from its name.

> Be warned:  
> For now, we store color tokens for apps in a [separate file](https://www.figma.com/design/6wRtU5WKyHv4NjifQtcQYC/%F0%9F%92%A0-Core-Library-%5BApps%5D-%F0%9F%93%B1?m=auto&node-id=0-1&t=JuaWSrVDdeoSHxIq-1), due to differences between platforms. They will be merged in the future.

---

# Primitives, Semantics, and Components

Conceptually, Welcome’s new color system has three layers: primitives (also called raw colors), semantics (sometimes known as aliases), and components.

> Some extra info:  
> ⁉️ Not sure what this means? You can learn more about Design Tokens in this helpful [article](https://uxdesign.cc/design-tokens-cheatsheet-927fc1404099).

- Primitives are the base level of color. They connect a name — which could be a simple color name like “blue” or a branded name like “cerulean” — with a [perceived lightness](https://www.notion.so/Colors-4b0f7dfb68c74f5ca20a8f1134987a5a?pvs=21) index from 0 to 100, and a value in hexadecimal, HSL, or HCT format. For example, `wel&hyphen;prim&hyphen;color&hyphen;blue&hyphen;96` has the value `&num;F4F2FD`. These primitives aren’t meant to be used directly; rather, they form a pool of colors referenced by the semantic layer.

- Semantics are the second (and, in most cases, last) level of color. A semantic color reference (or alias) is a primitive and adds contextual information on the purpose of the color. As much as possible, users need to be able to know how to use a color only by reading its semantic name. An example of a semantic is: `wel&hyphen;sem&hyphen;color&hyphen;on&hyphen;primary&hyphen;container` that refers to `wel&hyphen;prim&hyphen;color&hyphen;neutral&hyphen;15` in its value.

- Components are the third and final level of color. They refer to semantic tokens and provide information related to a specific component. For instance, `wel&hyphen;comp&hyphen;btn&hyphen;primary&hyphen;fg&hyphen;color` refers to `wel.web.bComp&hyphen;btn&hyphen;primary&hyphen;light&hyphen;fg&hyphen;color` in its value. We take care to avoid enriching this third level to prevent unnecessary complexity.

# The HCT color model

The color system in Welcome is based on [Google’s attempt](https://material.io/blog/science-of-color-design) to create a perceptually accurate color space. In this system, color is described using three main parameters:

- **Hue** (H) represents the shade of color along the circular rainbow scale, which ranges from 0 to 360.

- **Chroma** (C) is the saturation of the color, measured between 0 and 145.

- **Tone** (T) is the most important parameter. It indicates the color’s perceived lightness from 0 (black) to 100 (white).

> Some extra info:  
> [Perceptually accurate color systems](https://programmingdesignsystems.com/color/perceptually-uniform-color-spaces/) adjust lightness so it’s not influenced by hue. For example, yellow naturally appears brighter than red at the same lightness level. In this adjusted space, yellow is made slightly darker and red slightly lighter to better match other colors.

All of Welcome’s primitives use the HCT model. This model has one advantage over others like Oklab and Cielab: it incorporates [WCAG color contrast requirements](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html).

To meet WCAG AA contrast standards, paired colors need a contrast ratio of at least 4.5:1 for text or 3:1 for non&hyphen;text elements. Usually, this test is checked using plugins or specialized websites.
With HCT, a simple look at the color’s indices guarantees contrast ratios:

- An index gap of 30 or higher means a 3:1 ratio.

- An index gap of 50 or higher means a 4.5:1 ratio (WCAG AA)

- An index gap of 70 or higher means a 7:1 ratio (WCAG AAA)

Keep in mind, since hue affects contrast, a color&hyphen;10 paired with color&hyphen;60 may not always have the exact ratio. However, HCT guarantees it will always be above 4.5:1.

# Figma structure

All colors are stored in a single source of truth in Figma, 🌈 **[platform name] Appearances**

![Img](https://studio-assets.supernova.io/design-systems/161625/8efa8b75-cb0d-46ff-bbe3-5d2886940ddf.png)

In the future, we will implement a single source of truth (SST) to share variables effortlessly across platforms like web and mobile.

> Be warned:  
> When designing, make sure that your file is connected with **🌈[platform] Appearances** libraries.

# The color system

## Parameters

Creating a semantic color system means describing color using concepts beyond just the color itself. When designers pick a color, they often rely on unwritten rules learned through experience. A semantic system writes those rules down so that, in the same context, different designers will make the same color choices.

These concepts shape interface design and include questions like:

- What element is the color applied to? Is it a border, a background — and if so, what kind of background — text, an icon, etc.?

- What is the UX function of the element? Does it convey meaning like information, warning, or error?

- What is the technical affordance of the element? Is it static or interactive? What is its current state?

- What hierarchy level does the element have within the page or among elements of the same type?

- What theme, brand, or sub&hyphen;theme is applied to the element?

Of course, using all these parameters to name color tokens would create very long names and too many variables. In Welcome’s color system, we find a balance between simple naming and precise, controlled usage.

Material’s color system uses these parameters:

- **Emphasis: **The importance level of the element within the page or product. Primary is the highest, followed by Secondary and Tertiary. Within those, there’s a distinction between default color (like `primary`) and Container variants (like `primary&hyphen;container`).

- **Element: **The object the color applies to — such as Surface (page or section background), Container (a subdued background that’s not a page or section), Outline (border), or Overlay.

- **Function: **The UX purpose the color serves. This can be a general interface function like Danger, Success, or Warning, custom functions like Link, Accent, Inverse, or brand&hyphen;specific functions like Loyalty and Offer (for the All theme).

- **Level: **The hierarchy within the token family, with levels ranging from min, low, mid, hi, to max.

- **Relationship: **If a color is applied on top of another color, it can be named with an “on” prefix, such as `on&hyphen;primary`.

> undefined  
> Not all parameters are used in every color name. For example, `primary&hyphen;container` uses emphasis and element, while `warning` only uses a function because it applies across all element types. Also, Material includes implied rules not always explicit in names — for example, Container usually indicates lower emphasis than its related color. These rules will be explained further in this documentation.

> Some extra info:  
> 

## Surfaces

Surfaces are the foundational colors used in our interfaces. They support the elevation system.

- The `surface`** **color is the default background for pages or sections. It contrasts with all text colors and with other non&hyphen;surface colors to maintain clear visibility for non&hyphen;text elements.

- `surface&hyphen;container`** **is a variant of the surface color with five gradient levels: min, low, mid, hi, and max. You can use it for any background to create visual hierarchy and elevation.

- `on&hyphen;surface`** **colors are the default text colors. They apply only to text and icons and come in three levels: low, mid, and high.

- `success&hyphen;container`, `warning&hyphen;container`, and `danger&hyphen;container `are available to create surfaces with a function (see below).

> Be warned:  
> Note that text and icons share the same color considerations because icons often accompany text. If we need guidelines for illustrative icons, we will provide them separately.

> Some extra info:  
> 

## Main colors

These are the brand colors. You can have up to three, ordered by emphasis: primary, secondary, and tertiary. Each color comes with a paired color that uses the **on&hyphen; **prefix, as well as a Container variant. For example:

- `primary` is the main brand color. Use it on any high&hyphen;emphasis UI element, except for surfaces like section and page backgrounds.

- `on&hyphen;primary` is the contrasting color paired with `primary`. It is mainly used for text and icons. Exceptionally, it can also be used as a background in complex layouts.

- `primary&hyphen;container` is a lower&hyphen;emphasis variant of `primary`. Because it has less emphasis, it does not meet text contrast requirements against surfaces, so use it only as a background for elements containing text (when layered on top of a surface). However, it can be paired with `primary` for non&hyphen;text elements where a 3:1 contrast ratio is enough.

- `on&hyphen;primary&hyphen;container` is the paired color to be used only on text and icons.

> undefined  
> The same structure applies to secondary and tertiary colors.

## Function colors

ur color system includes a selection of colors that communicate clear messages:

- **Standard web feedback colors**: `danger` (red), `warning` (orange), and `success` (green).

- **Custom feedback colors**: `link` and `focus`.

- **Transversal brand colors**: `loyalty` and `offer`.

The first three — danger, warning, and success — are straightforward and follow the same family structure as the main colors. The others have their own specific features:

- `link`** **(used for links) and `focus`** **(used for focus outlines).

- `loyalty`** **and `offer` follow the same family structure as the main colors.

## Context colors

Lastly, all colors are available for specific contexts:

- `outline`** **is dedicated to container borders and comes in two variants:

- `outline&hyphen;[function]` tokens, e.g., `outline&hyphen;warning`, are dedicated to each function container border.

- `overlay&hyphen;hi`** **and `overlay&hyphen;low`** **are designed for overlays, such as those used in modals.

## States

Color is a key way to show state changes like hover, focus, pressed (or touched on mobile), active or selected, and sometimes disabled.

### Interaction states

Colors usually have 3 state variants when appropriate:

- **Hover**: used for hover states.

- **Pressed**: used for the pressed or active state on the web (when an element is clicked). This variant can also represent the “visited” state on links.

- **Focus**: has its own distinct color and behavior.

Other states, like active and selected, use colors on a case&hyphen;by&hyphen;case basis. We’ll provide a detailed guide on interaction patterns soon to help you signal interactions consistently.

### Disabled state

Welcome’s color system does not include specific disabled colors (such as grey&hyphen;muted tones). Instead, a consistent method is used across components to indicate the disabled state: applying 38% opacity to the component.

- `outline&hyphen;hi` for important or interactive borders that maintain a 3:1 contrast with all surfaces.

- `outline&hyphen;low` for decorative borders and dividers.