
# Picking colors

---

# Finding the right token

Thanks to how our system is designed around what each color represents (see [Parameters](./overview.md) above), choosing the right color for any context comes down to asking a few simple questions, outlined in the decision tree below:

![Img](https://studio-assets.supernova.io/design-systems/161625/623cb4ea-4378-4383-82eb-943acc28f000.png)

Migrating colors from the legacy system? [Find a matching table.](https://docs.google.com/spreadsheets/d/1m0uEkZxEsM2zDEXhqrDQCuH1B_Cz_WIrj_OQloaPcUw/edit?gid=358923631#gid=358923631)

# Building a theme

One of the key strengths of Welcome’s color system is its support for multiple brand themes while maintaining a single Design System. This is made possible thanks to Figma’s variable feature and CSS theming capabilities on the code side.

> Some extra info:  
> Learn more about Welcome’s theming architecture and governance [in this file](https://www.figma.com/design/78PLAbZPNx1h6kyNsYtCpT/Theming-Demo?node-id=7-9753&t=W8h4soZAjX2Raekc-11).

Because every theme must be pre&hyphen;built in our Figma files, and semantic color names are shared across all themes, we use a method explained below.

## Creating the color ramps

Let’s imagine a new brand called Banana that needs to be added to the Design System’s theming options. It comes with the following colors:

  
![Brand colors](https://studio-assets.supernova.io/design-systems/161625/5d73fcf6-a4cb-4132-8dab-e2951f1da60a.png)  
Brand colors  


The first step is to create **color ramps** for each brand color. This means generating a scale of color variants ranging from black (tone = 0) to white (tone = 100).

To do this, we use the [Material Theme Builder](https://material-foundation.github.io/material-theme-builder/). We keep the brand’s reference color (marked with a star) in the ramp, while aiming to maintain consistent values outside that specific color. If the brand’s colors don’t have a clear hierarchy, we assign them based on their most logical use.

For example, the dark blue can serve as an accent color (alternative high emphasis), while the pink or grey colors can function as neutral (default) colors.

  
![Ramps](https://studio-assets.supernova.io/design-systems/161625/f4f4ebac-c7dd-4023-9bea-0f7953025ee3.png)  
Ramps  


## Choosing the main colors

Now it’s time to select which index from the color ramp will be used for the variants within a color family. As explained earlier, each color family can have up to four variants: the main color and its pair (`on&hyphen;color`), plus the lower&hyphen;emphasis variant (`color&hyphen;container`) with its respective pair `on&hyphen;color&hyphen;container`).

Accessibility requirements and color usage contexts guide our choice of index. For example, main colors can be used on text or backgrounds (excluding surfaces). To meet WCAG text contrast standards against any surface, the color must have an index gap of 50 or more compared to the darkest surface (see the [HCT model](https://m3.material.io/styles/color/system/how-the-system-works) for details).

To maintain flexibility, we limit surfaces in light mode to tones between 90 and 100. This means the main colors must have an index of 40 or less (90 minus 50) to qualify.

In our case study, the brand’s main color has an index of 56, so it cannot serve as the `primary` semantic token. However, the lower&hyphen;emphasis variant, `primary&hyphen;container`, doesn’t face this restriction since it’s used only for backgrounds.

> undefined  
> If the brand’s main color had an index <40, we would use it directly as the primary color, though this is less common.

That gives us our first semantic color: `primary&hyphen;container`, which directly uses the brand’s main color at index 56.

  
![First](https://studio-assets.supernova.io/design-systems/161625/479e7d47-4a6e-49d0-8c6d-d24ea70c5d87.png)  
First  


Next, we select the `primary` color by considering its pairing constraints with the `primary&hyphen;container`. These need to maintain a minimum 3:1 contrast ratio for non&hyphen;text elements, meaning an index gap >30. This guides us to choose colors with an index of 26 or lower. For this example, we’ll go with `mud&hyphen;25`.

  
![Second](https://studio-assets.supernova.io/design-systems/161625/fd09662d-4667-4bd4-bb16-762014981f2a.png)  
Second  


Pairings designed for text require a higher contrast ratio of 4.5:1, which means a minimum index difference of 50. To achieve this, we add a color at index 6 to the mud color ramp (56 minus 50), resulting in a suitable pair.

  
![Last](https://studio-assets.supernova.io/design-systems/161625/517e055e-603b-49b6-97dc-a28d54e307c1.png)  
Last  


You can follow the same process with other color families. For example, `secondary` with the Cream ramp, accent with Navy, and so on. Neutral colors don’t form their own family but use colors like Lilac to create `surface`, `surface&hyphen;container`, and `on&hyphen;surface`** **colors.

  
![Frame 80](https://studio-assets.supernova.io/design-systems/161625/58ed07ad-682b-4f97-9286-6b727460a1e0.png)  
Frame 80  


> Some extra info:  
> If a theme doesn’t specify a particular color, it defaults to the value defined in the default theme of the Design System, representing All.com’s visual identity.

## Color constraints

When choosing light colors, the main rule is that surfaces should have a tone index of 90 or lower. For dark mode, the rule flips: surfaces need a tone index of 20 or higher. This difference comes from how we perceive contrast non&hyphen;linearly across the color ramp.

> Some extra info:  
> What does “non&hyphen;linear contrast” mean? On a color ramp, you need a bigger index gap to achieve the same perceived contrast in the darker range compared to the lighter range. While Material’s HCT model already adjusts indexes to consider this, we still need to pick different index gaps for light and dark modes.

For example, in light mode, visible contrast for text on surfaces requires using colors from `grey&hyphen;10` to `grey&hyphen;40`. But in dark mode, you can achieve the same visual hierarchy using colors from `grey&hyphen;85` to `grey&hyphen;100`.

Taking this into account, here are the full index rules for color choices:

  
| Column 1 | Column 2 | Column 3 | Column 4 |  
| --- | --- | --- | --- |  
| Semantic color | Indexes (Light) | Indexes (Dark) | Contrast needs |  
| **Surfaces**<br>`surface` and all `surface&hyphen;container` variants | 92&hyphen;100 | 0&hyphen;20 | 4.5:1 with all main colors<br>4.5:1 with all `on&hyphen;surface` colors |  
| **All main and functional colors**<br>`primary`, `secondary`, `accent`, `danger`, `warning`, `success`, `loyalty`, etc. | 0&hyphen;40 | 70&hyphen;100 | 4.5:1 with all `surface` colors<br>3:1 with corresponding `container` color<br>4.5:1 with corresponding `on&hyphen;` color |  
| **Lower emphasis**<br>“container” colors (e.g., `primary&hyphen;container`, etc.) | 30&hyphen;92 | 20&hyphen;70 | Should be different from all `surface` colors<br>4.5:1 with corresponding `on&hyphen;` color<br>3:1 with the corresponding main color |  
| **On&hyphen; pairing** for main colors (e.g., `on&hyphen;primary`) | 50&hyphen;100 | 0&hyphen;50 | 4.5:1 with the corresponding main color |  
| **On&hyphen; pairing** for “container” colors (e.g., `on&hyphen;primary&hyphen;container`) | 0&hyphen;100 | 0&hyphen;100 | 4.5:1 with corresponding container color |  
| `on&hyphen;surface` color family | 0&hyphen;40 | 70&hyphen;100 | 4.5:1 with all `surface` colors |  
| `outline&hyphen;hi` | 0&hyphen;60 | 50&hyphen;100 | 3:1 with all `surface`colors (to achieve non&hyphen;text contrast for interactive elements) |  
| `outline&hyphen;low` | 0&hyphen;90 | 20&hyphen;100 | Shouldn’t be any `surface` color |  
