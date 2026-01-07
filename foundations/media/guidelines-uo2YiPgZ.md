
# Guidelines

---

# Designing with ratios

## Custom proportions

As a designer, you can set Media items to custom proportions using the **Media&hyphen;Free **variant. These can be static or dynamic. Static items keep the same size regardless of screen size. For example, an image with fixed dimensions of 200×300 pixels.

  
![Static](https://studio-assets.supernova.io/design-systems/161625/c76549ac-6d35-42cc-9681-0253e7738a10.png)  
Static  


Dynamic custom dimensions mean the Media item grows relative to its container or a portion of it. For instance, a hero image that spans 100% of the viewport’s width but maintains a fixed height. In such cases, use **Media&hyphen;Free**.

  
![Dynamic](https://studio-assets.supernova.io/design-systems/161625/4774ee9a-ede9-4954-b582-930aba5cc679.png)  
Dynamic  


> Be warned:  
> Be cautious with dynamic dimensions, they can cause distortion or cropping. Use CSS `object&hyphen;fit: cover` to prevent content stretching and carefully select content to avoid important details being clipped. On AEM, these issues are rare since CMS contributions don’t always guarantee the content beforehand.

## Strict ratios

Another option is to use Media items with fixed aspect ratios by using the **Media&hyphen;Fixed **variant. Ratios can change at different Breakpoints: a taller aspect ratio is recommended on mobile, while wider ones suit desktop. 

For example, an image could be 3/2 on `desktop medium` and `desktop small`, 1/1 on `tablet`, and 8/10 on `mobile`. Between Breakpoints, the ratio is maintained, so Media grows proportionally.

  
![Strict](https://studio-assets.supernova.io/design-systems/161625/2cfdc3ef-cb0f-4eea-9f4e-d81cef2c4f92.png)  
Strict  


## Mixed behavior

Another option is to use Media items with fixed aspect ratios by using the **Media&hyphen;Fixed **variant. Ratios can change at different Breakpoints: a taller aspect ratio is recommended on `mobile`, while wider ones suit `desktop medium`. 

For example, an image could be 3/2 on `desktop medium` and `desktop small`, 1/1 on `tablet`, and 8/10 on `mobile`. Between Breakpoints, the ratio is maintained, so Media grows proportionally.

  
![Mix](https://studio-assets.supernova.io/design-systems/161625/07d5d013-99da-4851-82eb-ae4faf414225.png)  
Mix  


> undefined  
> To create this, use **Media&hyphen;Free **and set the right dimensions and resizing constraints.

# Fallback content

A fallback color is mandatory for images that fail to load or display for any reason.

This fallback color is the inverse.

The brand logo is also displayed, with its color set to `overlay&hyphen;low`.

  
![Carousel with the fallback display instead of images.](https://studio-assets.supernova.io/design-systems/161625/49d473f3-f1fc-44c2-8f99-ab7bfc032ef8.png)  
Carousel with the fallback display instead of images.  


# Corner radius

By default, Media has a corner radius of 0px. In the ALL theme, it’s recommended to use the default radius (`radius&hyphen;sm`) unless Media is embedded in a component that manages its own corner styling.

# Accessibility overlays

Media properties allow toggling scrim overlays, which are required when content is overlaid on images:

- **Overlay **adds an `overlay&hyphen;low`** **background between the image fill and overlaid content. Use this when adding non&hyphen;text elements or nested text elements (like Badges or Logo Slot) on Media. This option isn’t available for videos.

- **Overlay+ **adds an `overlay&hyphen;mid`** **background, ideal for adding text directly on images. For videos, this is the default to keep elements like the play icon visible.  

  
![Overlays](https://studio-assets.supernova.io/design-systems/161625/1f467817-2b3c-4bcd-9969-b26377551ef7.png)  
Overlays  


> Be warned:  
> Always set any content added on Media to [local dark mode](../color/guidelines.md).

# Text alternatives

Add text alternatives to images for assistive technologies:

- Captions can be added directly in the Figma component and are visible to all users.

- Alternative text (HTML `alt`) should be specified for every image in your designs, which you can annotate in Dev Mode for handoff.

  
![Captions](https://studio-assets.supernova.io/design-systems/161625/c348d4b1-e284-484a-b35e-8990ab1d618a.png)  
Captions  
