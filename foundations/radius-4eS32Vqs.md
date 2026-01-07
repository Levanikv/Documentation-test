
# Radius

Create rounded corners with border radius tokens.

---

Border radius tokens define the corner rounding applied to UI elements across all Accor brands. They ensure visual consistency while allowing brand&hyphen;specific customization. The token system is organized hierarchically, from semantic tokens that express intent to component&hyphen;specific tokens for specialized use cases. Here is the list of available Tokens.

  
surface: 6px  
container-low: 6px  
container-high: 6px  
input: 6px  
static-sm: 2px  
static-md: 4px  
static-lg: 6px  
interactive-low: 12px  
interactive-high: 100px  
full: 100px  


# Semantic Border Radius Tokens

Semantic tokens express the purpose of the border radius rather than its value. This approach enables brand theming while maintaining consistent application logic.

## Surface

**Token path: **`wel.sem.borderRadius.surface`

Use this token for large background containers such as [Modal](#), [Popin](#), [Drawer](#) and page&hyphen;level panels. Surface elements provide the foundational visual layer of the interface.

## Container Low

**Token path: **`wel.sem.borderRadius.container&hyphen;low`

Use this token for structural wrappers and layout blocks with low visual emphasis such as [Card](#), [Image Product](#), [Skeleton](#) and [Slideshow](#). These containers organize content with a low visual emphasis.

## Container High

**Token path: **`wel.sem.borderRadius.container&hyphen;high`

Use this token for floating, interactive, or high&hyphen;emphasis containers such as [Date Picker](#), [Selector](#), [Link](#), [Message](#), [Snack Bar](#) and [Tooltip](#). These elements typically overlay other content or require visual prominence.

## Element Static

Static element tokens apply to non&hyphen;interactive UI elements that display information without user interaction.

### Static Small

**Token path: **`wel.sem.borderRadius.element.static&hyphen;sm`

For small static elements where minimal rounding provides visual refinement such as [Icon Slot](#)

### Static Medium

**Token path: **`wel.sem.borderRadius.element.static&hyphen;md`

For default&hyphen;sized static elements that benefit from moderate corner rounding such as [Countdown](#), [Badge](#) and [Badge Counter](#).

### Static Large

**Token path: **`wel.sem.borderRadius.element.static.lg`

For large static elements such as icons and logos at prominent sizes such as[ Logo slot](#)

## Element Interactive

Interactive element tokens apply to components that respond to user input. The radius level communicates the emphasis and importance of the action.

### Interactive Low

**Token path: **`wel.sem.borderRadius.element.interactive&hyphen;low`

For interactive elements with low emphasis, such as selectable components or secondary actions such as [Chip](#) and [Segmented Control](#). Typical values create pill&hyphen;shaped or moderately rounded appearances.

### Interactive High

**Token path: **`wel.sem.borderRadius.element.interactive&hyphen;high`

For primary interactive elements such as [Button](#). This token defines the most visually prominent interactive style.

## Element Full

**Token path: **`wel.sem.borderRadius.element.full`

Use this token for absolutely round UI elements where brand customization is not applicable such as Map Pointer, [Icon Button](#), [Stepper](#), [Autocomplete](#), [Avatar](#) and [Toggle](#). These elements always render as perfect circles or pills regardless of theme.

## Input

**Token path: **`wel.sem.borderRadius.input`

A dedicated token for all form input elements such as [Input Currency](../web/core-components/input-currency/overview.md), [Input Phone](../web/core-components/input-phone-number/overview.md) and [Input Text](#). This ensures consistent styling across text fields, dropdowns, and other input types.

# Component&hyphen;Specific Tokens

Some components require dedicated tokens due to their unique visual requirements or specialized context. Use these tokens only for their designated components.

## Map Pointer

**Token path: **`wel.comp.mapPointer.radius`

Defines the border radius for map pins displaying hotel rates. Consider aligning with element.static&hyphen;md for consistency across the system.

## Booking Engine

**Token path: **`wel.comp.bookingEngine.radius`

Defines the border radius for the Booking Engine wrapper. This high&hyphen;visibility component may warrant distinct treatment per brand.

## Checkbox

**Token path: **`wel.comp.checkbox.radius`

Defines the border radius for the checkbox.