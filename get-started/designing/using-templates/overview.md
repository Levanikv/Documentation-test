
# Overview

---

Templates can be found in the file. As of now, Templates are only available for Web pages, but we might add similar tools for Apps (some pre&hyphen;populated App pages are available [here](https://www.figma.com/design/wUPdTa0EP52i6pRhA0Yaco/%F0%9F%93%B1-Welcome-Library-%5BApp%5D?node-id=55-39768)).

You can find Templates in the [Helpers](https://www.figma.com/design/8rXIFNeQKCUcRUa1twTfJJ/%F0%9F%A7%B0-Helpers?node-id=779-22526&t=n4VANUqFF2HSVVPP-1) file. Currently, Templates are available only for web pages, but similar tools for apps may be added in the future. Some pre&hyphen;filled app pages are available [here](https://www.figma.com/design/wUPdTa0EP52i6pRhA0Yaco/%F0%9F%93%B1-Welcome-Library-%5BApp%5D?node-id=55-39768).

# Structure

  
![Page](https://studio-assets.supernova.io/design-systems/161625/4a003904-cf74-468f-b5ab-dd3f0ee2112a.png)  
Page  


Templates are built as stacks of empty boxes organized as follows:

- At the top is the **Header (1)**, with a default gap of zero. It houses top components like Heading Page, Navigation, and Quick Access.

- The middle contains a frame for the **Page (2)**, which manages top and bottom margins using `afterHeader`** **and `beforeFooter`.

- Inside the Page are two Sections by default (more can be added by copying and pasting). Sections are spaced using `withinPage`, with an internal gap of `withinSection&hyphen;md`.

- At the bottom is a frame dedicated to footer components, mainly the **Footer (3)**.

[Learn more about page spacing](#).

> undefined  
> Templates also offer optional UI mockups for popular operating systems and browsers.

# Sections

Sections are the core building blocks of page content:

- Each Section typically starts with a title, like an AEM Heading Section.

- You can insert any AEM component directly inside a Section. Core Components require a wrapper (please see the [Guide](./guide.md)).

- There are two Section types:

# Responsive

Templates support 4 Breakpoints and are fully responsive thanks to variable modes. This means once you configure a page with Templates, you can switch dynamically between Breakpoints — no need to create separate pages for each size.

With variable modes, all components and variables adapt automatically to the chosen Breakpoint, adjusting layout, spacing, text size, and more.

> Be warned:  
> Templates do not handle side margins. These are managed directly by components in AEM or should be added to wrappers when inserting Core Components.

If you want, the Design System Team can help you get started with Templates or show you how to make the most of their responsive features.


- Default Sections: no background, no margins

- Background Sections: a grey&hyphen;colored background (by default) with top and bottom margins