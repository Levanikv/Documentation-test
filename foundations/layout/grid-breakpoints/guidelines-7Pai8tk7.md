
# Guidelines

---

# For web designers

Designers, you may need to create mockups for the four main breakpoints, ranging from Mobile to Desktop medium. Components with responsive behavior typically either have variants for each breakpoint or adjust dynamically based on size.

In Figma, breakpoints aren’t a native concept. Instead, we replicate them using variables tied to Frame widths. To better represent average device sizes, the values at which Figma switches breakpoints are sometimes set in the middle of a range instead of the beginning:

- Mobile: 375px instead of 320px

- Tablet: 768px

- Desktop small: 1024px

- Desktop medium: 1340px instead of 1280px

> undefined  
> If you need to create mockups for larger breakpoints, remember that page content doesn’t change after 1280px, only the margins do. To design for Desktop Large and Extra Large, simply extend the parent Frame while keeping the content centered.

# For app designers 

You are expected to create mockups for five screen sizes, adapted to the specific needs of iOS and Android devices:

- iOS: 375px, 834px, 1210px  

- Android: 360px, 1440px  

In Figma, the concept of “Breakpoints” is replaced by “Screen Size” to reflect these values. Components should either have variants for each screen size or adjust dynamically to fit the layout. You may also need to specify the platform (iOS or Android) in the design properties to handle platform&hyphen;specific adjustments.