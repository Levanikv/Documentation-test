
# Guide

---

## Choosing a reference Breakpoint

Because Templates are responsive, you only need to design your page at one Breakpoint:

- When using only Design System components.

- When using local components that have four Breakpoint variations — `mobile`, `tablet`, `desktop small`, and `desktop medium` — just like Design System components.

The first step is choosing a reference Breakpoint at which we’ll design the page, e.g., `desktop medium`.

## Inserting a Template

Next, insert the Template as you would any regular component published from Helpers:

1. Open Figma Assets.

1. Add the Helpers library if it’s not already available.

1. Drag and drop the 🧰 Template from the Template page.

1. Select your chosen reference Breakpoint using the ‘breakpoint’ property.

  
![Insert](https://studio-assets.supernova.io/design-systems/161625/544a86c9-bb16-4add-9ad6-9b7b38018397.png)  
Insert  


From the properties panel, you can toggle the system UI visibility using the ‘top UI’ and ‘bottom UI’ boolean properties. After detaching the Template, you’ll manage these settings through the layers panel.

## Adding components

> Be warned:  
> The first step is to detach the 🧰 Template instance so you can add components. Remember, Templates are published as components to make them easy to find, but they aren’t components themselves. 

Components from the Core AEM library are optimized to work seamlessly with Templates and offer:

- Full viewport width with no resizing needed.

- Variants are available for different Breakpoints.

- Side margins when needed.

Core AEM components fall into three categories, as noted in their descriptions:

- **Header** components go in the Template’s top section.

- **Sections** can be added directly within the Template’s Page frame.

- **Components** are inserted inside Section frames available within the Template.

Let’s start designing by inserting our Heading Page. In the Assets panel, find Heading Page.

  
![Heading](https://studio-assets.supernova.io/design-systems/161625/694049c6-14b6-48cb-a43e-fc62ffa794df.png)  
Heading  


Drag and drop the component inside the Template, placing it in the frame named **header**.

  
![Inserted](https://studio-assets.supernova.io/design-systems/161625/45c30423-f839-403a-8d6d-b573f4644cd2.png)  
Inserted  


Next, configure the component to dynamically adjust to its parent’s frame mode:

1. Set the component’s mode to **Auto **(it defaults to **Mobile **).

1. Bind the component’s **breakpoint **property to the **breakpoint **variable from the 🌈 [platform] Appearances Library.

  
![Setting the mode](https://studio-assets.supernova.io/design-systems/161625/5e88ad64-f52d-4d55-a0c4-1133be697ece.png)  
Setting the mode, In the appearance tab  
  
![Binding variables](https://studio-assets.supernova.io/design-systems/161625/c537f88e-fd01-4917-a9f6-78a4cc16de7b.png)  
Binding variables, in the breakpoint property of your component  
  


> undefined  
> You’ll need to repeat these steps for any other components inserted from Core AEM.

### Other libraries

To insert components from other libraries (such as Core Components, Candidate, or local files), wrap them in a container that fills 100% of the viewport. Then, insert this wrapper inside a [Section](./guide.md).

[Find all viewport sizes](../../../foundations/layout/grid-and-breakpoints/breakpoints-web.md).

> Be warned:  
> To make sure your inserted wrappers work with Breakpoints, try and design them at 4 Breakpoints like design system components.

## Creating Sections

[Sections](./overview.md) are the containers inside the Page frame of Templates. By default, one section of each type (default and background) is available in the Template. To add more:

- Copy and paste an existing section (Figma frame).

- Or insert a section instance from Core AEM, then detach it to add components inside.

  
![Sections are Figma frames](https://studio-assets.supernova.io/design-systems/161625/70a0c89e-1c4b-46d8-91df-ab08c21c3ac0.png)  
Sections are Figma frames, Here, a Template with 2 Sections.  
  


## Switching Breakpoints

After designing a Template with components [as described above](./guide.md) (or even before, if you’ve bound components to the `breakpoint` variable), you can switch Breakpoints directly on the frame to preview your design at the 4 standard screen sizes.

  
![Breakpoint switch](https://studio-assets.supernova.io/design-systems/161625/42d0738c-fc29-491d-903b-a9184982f884.png)  
Breakpoint switch, Using Figma variable modes.  
  
