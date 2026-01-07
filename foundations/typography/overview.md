
# Overview

---

# Summary

As a single source of truth for text content, the typography Foundations offer a wide range of options to style text in various contexts. It matches the following requirements:

- **A platform&hyphen;agnostic naming convention**, designed to be used across all platforms, including iOS and Android.

- **A responsive system** that adjusts text styles based on screen size, without relying on designers to match desktop and mobile styles manually.

- **A themable system** that provides one list of styles with display modes tailored for each brand.

- **A simple yet versatile typescale**, with naming that avoids direct references to weight (like `bold` or `regular`) or size values.

> undefined  
> Like most semantic tokens, typography variables for web and app platforms are currently separate. Our future goal is to merge them into a single unified system.

---

# Composite tokens

Like some space tokens, typography styles are composite tokens. This means a token (or style, in Figma) combines several variables that describe every property applied to the text. Below is a list of possible variables you’ll find in a style token:

- **Font size: **the size of the letters

- **Font weight: **the visual thickness of the letters

- **Font family: **the font used

- **Line height: **the distance between two lines of text in the same style

- **Paragraph spacing: **the space between paragraphs or blocks of text sharing the same style

- **Letter spacing: **the horizontal gap between letters within words

- **Text case:** property in CSS is used to control the capitalization of text. It allows you to transform text to `uppercase`, `lowercase`, `capitalize` the first letter of each word, or leave it unchanged.

- **Text decoration:** is used to set the appearance of decorative lines on text. It is a shorthand for `text&hyphen;decoration&hyphen;line`, `text&hyphen;decoration&hyphen;color`, `text&hyphen;decoration&hyphen;style`, and `text&hyphen;decoration&hyphen;thickness`.

- …and others (see [CSS text properties](https://developer.mozilla.org/fr/docs/Web/CSS/text-align) for more details)

> Some extra info:  
> In most cases, **not all variables need to be specified in text styles** because they inherit default values from the browser, page, template, or theme. Typically, only the primary variables — font size, line height, and font family — vary between styles.

# Figma implementation

[🌈 Web Appearances](https://www.figma.com/design/HXpmNTzVqJhYs57bt2UJ11/%F0%9F%8C%88-Web-Appearances?m=auto&node-id=2408-2273&t=ToUyyFnZ563ZN4In-1) stores all typography variables and the 4 necessary typography modes: `mobile (320&hyphen;767)`, `tablet (768&hyphen;1023)`, `desktop&hyphen;sm (1024&hyphen;1279)`, and `desktop&hyphen;md (1280&hyphen;1439)`.

> undefined  
> The base variables are not intended for direct use but are available for exploration when creating new text styles. In most cases, we recommend using the predefined text styles.