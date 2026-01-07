
# Shadow and Background Blur

Create a visual elevation for components over the base page level.

---

# Styles

**Shadow tokens **are composite tokens, similar to Typography. In Figma, they are published as styles and use underlying variables to support theming.

  
default-up: 0px -2px 6px 0px rgba(0, 0, 0, 0.05)  
default-bottom: 0px 2px 6px 0px rgba(0, 0, 0, 0.05)  
strong-bottom: 0px 2px 6px 0px rgba(0, 0, 0, 0.2)  
default-up: 0px -2px 6px 0px rgba(0, 0, 0, 0.05)  
strong-up: 0px -2px 6px 0px rgba(0, 0, 0, 0.2)  
wide: 0px 8px 16px 0px rgba(0, 0, 0, 0.05)  


Each property composed to create the Shadow can be defined as it's own Token and referenced within the Box Shadow Composite Token**:**

- **X (untokenized)**

- **Y**

- **Blur**

- **Spread (untokenized)**

- **Shadow color**

  
**Y**  
  
shadow-up-y: -2px  
shadow-down-y: 2px  
shadow-down-wide-y: 8px  
  
  
**Blur**  
  
shadow-blur: 6px  
shadow-wide-blur: 16px  
backgroundBlur: 96px  
  
  
**Shadow Color**  
  
shadow-default: rgba(0, 0, 0, 0.05)  
shadow-strong: rgba(0, 0, 0, 0.2)  
  


# Guidelines

Currently, Welcome does not have definitive guidelines for using shadows. Use shadows carefully, keeping in mind that **wider shadows indicate higher elevation**. Also, upward shadows should only be applied to bottom&hyphen;aligned components because the default light source on web pages is considered to come from above.