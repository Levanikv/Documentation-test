
# In Figma

---

# Components

Since visual appearance is often not enough to make out an element, certain conventions are in place in Figma to quickly recognize the origin and scope of the various components available in Welcome:

> undefined  
> ✏️ Name: {emoji} {prefix}.{component&hyphen;name}

## Emoji

An emoji is used before any other parameter in all Design System (DS) components. They are useful to measure DS compliance and map component use:

- 💠 → Core Components

- 🧩 → Local elements

- 🧰 → Helpers

[Learn more about DS compliance](https://www.notion.so/Test-DS-compliance-562f2463b4dd44ae93002b12a8683dfc?pvs=4)

## Prefix

A prefix is then added to show the platform and/or brand on which the component is available. In the case of the brand, since most brand components are only available on AEM, the prefix will show the brand.

### Design Tokens

`wel` → Welcome design system package name

`prim` → Primitive Tokens

`sem` → Semantic Tokens

`comp` → Component Tokens

### Core

- `web` → vue.js and legacy (former Components not yet migrated to vue.js)

- `aem` → Components available on AEM only

- `app` → App components (iOS and Android)

- `hot` → Hotel tools components

### Local

- `web` → vue.js and legacy (former Components not yet migrated to vue.js)

- `aem` → Components available on AEM only

- `app` → App components (iOS and Android)

- `crm` → Components available for Emailing only

- `hot` → Hotel tools components

- `mp` → Components available for Media Portal only (DAM)

- For brand&hyphen;specific components, use the brand code name (for instance, `fai` for Fairmont, `ibs` for Ibis, etc.)

## Casing

Use the casing convention of the platform for which the component is destined:

- Web → vue.js [kebab case](https://developer.mozilla.org/en-US/docs/Glossary/Kebab_case)

- iOS → [camel case](https://developer.mozilla.org/en-US/docs/Glossary/Camel_case) native rule

- Android → [pascal case](https://developer.mozilla.org/en-US/docs/Glossary/Camel_case) native rule

> Yay:  
> Example: on Web: `web.badge&hyphen;counter`, on iOS: `app.slideButton`, and Android: `app.SlideButton`

## Language

Always use English, and written out names (no abbreviations).

# Building blocks

When creating specifing building blocks for components in Figma, remember to make them hidden (or private) components with a `.` prefix.

## Structure component

- Name: `.base&hyphen;{component&hyphen;name}`

- You can use the [Flag from the Helpers](https://www.figma.com/design/8rXIFNeQKCUcRUa1twTfJJ/%F0%9F%A7%B0-Helpers?node-id=7-745&t=MEgc487QIZyM6b9y-1) file as a tag next to the component.

- Remember to [surface the properties](https://help.figma.com/hc/en-us/articles/5579474826519-Explore-component-properties) in the master component if needed.

## Content component

- Name: `.content&hyphen;{component&hyphen;name}`

- You can use the [Flag from the Helpers](https://www.figma.com/design/8rXIFNeQKCUcRUa1twTfJJ/%F0%9F%A7%B0-Helpers?node-id=7-745&t=MEgc487QIZyM6b9y-1) file as a tag next to the component.

- Remember to [surface the properties](https://help.figma.com/hc/en-us/articles/5579474826519-Explore-component-properties) in the master component if needed.

## Container vs wrapper

The need can arise to group Figma layers in parent layers:

- If the parent layer has more than one child, name it `container`.

- If the parent layer has a single child (can be useful to adjust position, or expose properties), name it `wrapper`.