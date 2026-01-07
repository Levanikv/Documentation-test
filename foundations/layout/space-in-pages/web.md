
# Web

---

# Overview

The `spacingDynamic.page` and `spacingDynamic.withinSection` tokens define standardized spacing values specifically for page&hyphen;level layout structure. These tokens ensure consistent vertical rhythm and visual hierarchy across different page sections and components.

## Token Structure

All page spacing tokens reference primitive dimension tokens using the `{positive&hyphen;X}` pattern, where X represents the pixel value. This maintains consistency with the broader design token system and enables easy maintenance when base spacing values need to be updated.

> Be warned:  
> Page space tokens are responsive, meaning their values adjust based on the screen size.

## Tokens

  
**Desktop (small and medium)**  
  
afterHeader: 56px  
withinPage: 56px  
beforeFooter: 48px  
2xl: 32px  
3xl: 48px  
4xl: 56px  
xl: 24px  
  
  
**Tablet & Mobile**  
  
afterHeader: 56px  
withinPage: 56px  
beforeFooter: 48px  
2xl: 32px  
3xl: 48px  
4xl: 56px  
xl: 24px  
  


## Standard layout

Page spacing tokens work best in standard layouts, which consist of:

- A top section called the **Header** (1).

- A content area called the **Page** (2), which includes sub&hyphen;elements called Sections.

- A bottom section called the **Footer** (3).

![Img](https://studio-assets.supernova.io/design-systems/161625/4a003904-cf74-468f-b5ab-dd3f0ee2112a.png)

> undefined  
> We understand that not all products or scopes follow this layout. However, page space tokens are designed to standardize most pages — starting with editorial content, often created in AEM — and provide flexible yet reliable guidelines for exceptions.

### Header

  
![header](https://studio-assets.supernova.io/design-systems/161625/1764f3d3-fd2b-40a8-a33f-53f6ae0669db.png)  
header  


The **Header** is the first section of every page:

- You can add components like Navigation, Heading Page (AEM), or any other component from the corresponding Figma section to it.

- By default, there’s no spacing inside the Header, but you can use `withinSection` tokens to add spacing as needed.

### Page & Sections

The Page sits in the middle, with its top margin controlled by `afterHeader`** **and its bottom margin controlled by `beforeFooter`. Both use default values in [Templates](../../../get-started/designing/using-templates/overview.md) but can be customized.

  
![body](https://studio-assets.supernova.io/design-systems/161625/7b847f8f-f7f6-4cd0-81df-545e8a9968d3.png)  
body  


Inside the **Page**, you’ll find **Sections**. The space between Sections is controlled by the `withinPage `token, which is unique to each theme. Within Sections, components can be spaced using four levels of `withinSection`** **tokens:

- `withinSection&hyphen;xl`** **is the most spacious and should be used sparingly, mainly for editorial sections. It usually matches the values of `withinPage`.

- `withinSection&hyphen;lg`** **is intended for primary sections.

- `withinSection&hyphen;md`** **is for secondary sections.

- `withinSection&hyphen;sm`** **is the most compact and suits minor sections.

> Be warned:  
> To maintain a clear visual hierarchy on the page, the largest `withinSection`** **value should always be equal to or smaller than `withinPage`. There is no strict rule for the smallest value.

To learn more about Section types,  check out the [Templates documentation](../../../get-started/designing/using-templates/overview.md).

### Footer

The Footer is the last section on the page. It usually only contains the Footer components (AEM or Pattern), but could also house other components.

  
![footer](https://studio-assets.supernova.io/design-systems/161625/295a00f4-d8fb-4674-a070-942978ca608f.png)  
footer  


Default spacing inside the Footer is zero, but can be customized when other components are added, using **withinSection **tokens.

# Titles

There are two scenarios to consider when working with **titles** in Welcome:

- In AEM, titles should only be created using specific components: **Heading Page **(for page titles, used once per page) and **Heading Section **(for section titles). These components have their own space tokens that should not be modified.

- Outside of AEM, titles can be created using the [Display and Title text styles](../../typography/overview.md). Think of titles as part of a section, and space them using `withinSection`** **variables.

# Guidelines

## Using Templates

The best way to follow space guidelines is to use Welcome’s ready&hyphen;made Templates, which are powered by variables.

Check out the [Templates documentation](#) for more details.

Templates are ideal for designing interfaces in AEM since they match Adobe’s CMS page structure, but they also work well for top&hyphen;level structures on any technical stack.

## Customization

Using space variables or their values is recommended, but not mandatory. You can override them as needed to suit your specific cases.

### Non&hyphen;section components

Most Core AEM and Core Patterns components are section&hyphen;level, meaning they can be placed directly within the Page or a Section. This usually means they span the full width of the page.

  
![With AEM components](https://studio-assets.supernova.io/design-systems/161625/5d516469-0c82-4f42-b0f8-524c71749363.png)  
With AEM components, Billboard (AEM) inserted directly in a Template section.  
  


You can still use lower&hyphen;level components while respecting page space guidelines by placing them inside a container that spans 100% of the page’s width. This can be done with or without using Templates.

  
![Core Components](https://studio-assets.supernova.io/design-systems/161625/342d5b9f-8a08-43d6-badd-a86ec16dc1a9.png)  
Core Components, Custom section made with Core Components and inserted in a Template section.  
  


### Stacking Sections

In the standard layout, Sections are spaced using `withinSection`** **tokens, which are implemented as gaps in Templates. 

![Img](https://studio-assets.supernova.io/design-systems/161625/5bf1a826-c14a-439a-a16e-073e9b6dc914.png)

However, in some cases, stacking Sections with no gap between them can create a better visual effect:

- When a Section with a background is followed by another Section with a background.

- When combining a Section with a background and components like Special Touches, which are entirely images.

In these situations, you can bypass `withinSection`** **spacing, typically by creating a parent frame with zero gap.

  
![Do](https://studio-assets.supernova.io/design-systems/161625/9d916d7e-8fcf-426a-ad49-967056654d80.png)  
Do  
