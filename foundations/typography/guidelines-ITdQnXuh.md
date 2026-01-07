
# Guidelines

---

# Picking a style

Typography styles cover all text needs across products:

- **Display **styles** **are recommended for page and section titles. They use fonts optimized for large sizes.

- **Title **styles are for component headings (Design System components and custom containers) and typically use a plainer font than Display styles.

- **Sub **styles** **complement subtitles and usually use an alternate font.

- **Body, Label a**nd **Caption **styles** **are used for body text and labels, with three levels of emphasis.
Please note, **Caption** is intended for fine print or non&hyphen;essential info since it’s very small and might be hard to read for users with disabilities.

- **Detail** style is dedicated to kicker elements.

- **Link** styles are dedicated to links.

- **Input **styles are used for input elements (input text, input password, chips, dropdowns..)

> undefined  
> Need a style for a specific context? Reach out to your DSM or use the Design System Requests channel on Teams.

# Decorating text

To change the appearance of text, several CSS properties are used (similar properties apply on other platforms):

- **Text&hyphen;decoration **adds underline, overline, or strikethrough.

- **Font&hyphen;style **applies italic.

- **Font&hyphen;weight **controls bold.

Going forward, the Design System recommends:

- **Underline is exclusively for links** and can be controled with the dedicated styles.

- **Bold, strikethrough, or italic are not for default use**. If needed, semantic styles can be added to tokens, similar to “strong” variants.

- For exceptions, Figma shortcuts like `CMD+I` (italic), `CMD+B` (bold), and `CMD+SHIFT+X` (strikethrough) can be used to add variations without detaching the style.