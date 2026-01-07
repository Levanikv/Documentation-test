
# Overview

---

# Introduction

Media is a transversal primitive that manages bare visual media files, including images and videos. In Figma, media is available as 2 components:

- **Media&hyphen;Fixed**, which locks the aspect ratio

- **Media&hyphen;Free**, which has no aspect ratio constraints

Code implementation varies but usually relies on native HTML tags like `<img>`.

# Aspect ratio

Depending on your platform, it’s often easier to work with images and videos using one of the predetermined ratios below:

- 11/5

- 13/5

- 16/5

- 16/9

- 1/1

- 3/2

- 4/3

- 6/5

- 8/10

Media items can be configured to behave in 1 of 3 ways:

- Using custom, designer&hyphen;defined proportions.

- Following strict aspect ratios.

- A combination of both. Ratios at Breakpoint thresholds with dynamic sizing beyond those points.

[You can learn more with examples in the Guidelines documentation](./guidelines.md)

On AEM, aspect ratios are built directly into components, following one of the three options above. For example, the Heading Page component has a fixed ratio set for each Breakpoint. Submit your images in a default ratio, and AEM will smartly crop them to fit other ratios as needed.

[Learn more about adding images to AEM](https://www.notion.so/AEM-media-DAM-contribution-104badc89751808c8643f7192c7f5747)