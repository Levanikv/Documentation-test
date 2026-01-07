
# Typography for iOS and Android

---

Typography plays a crucial role in creating a clear visual hierarchy and improving readability across all app interfaces. This guide presents the typography styles used in iOS and Android apps, ensuring consistency and accessibility on all screen sizes and devices.

# **Hierarchy**

Use these typography styles consistently to maintain a clear and accessible visual hierarchy throughout the app:

  
| Column 1 | Column 2 |  
| --- | --- |  
| **Typography Style** | **Usage** |  
| **display&hyphen;01** | Main headers on screens, typically for titles |  
| **display&hyphen;02** | Secondary headers |  
| **title&hyphen;01** | Section headings, or major content blocks |  
| **title&hyphen;02** | Subsection headers |  
| **subtitle** | Smaller subheadings or labels |  
| **body&hyphen;01** | Main body text for content |  
| **cta** | Call to action buttons and links |  
| **body&hyphen;02** | Secondary body text |  
| **body&hyphen;strong&hyphen;02** | Emphasized secondary body text |  
| **body&hyphen;03** | Tertiary text or small UI elements |  
| **body&hyphen;strong&hyphen;03** | Emphasized tertiary text |  
| **caption&hyphen;01** | Minor text, such as captions and disclaimers |  
| **caption&hyphen;strong&hyphen;01** | Emphasized captions or small text |  
| **caption&hyphen;02** | Minor text, such as captions and disclaimers |  
| **caption&hyphen;strong&hyphen;02** | Minor text, such as captions and disclaimers |  
| **chip** | Small compact labels, often upper captions |  
| **cta&hyphen;text&hyphen;link** | Text links with Call to Action behavior |  


  
![DO space typo](https://studio-assets.supernova.io/design-systems/161625/e2b3caf5-9141-4047-afae-0352aa4bbe04.png)  
DO space typo  


# **Font families and Styles**

Both iOS and Android apps use system fonts to ensure compatibility, performance, and accessibility across devices. Here’s a breakdown of the fonts used:

- **iOS**: SF Pro is used for all iOS interfaces. [Download SF Pro](https://developer.apple.com/fonts/)

- **Android**: Roboto is used for Android interfaces. [Download Roboto](https://fonts.google.com/specimen/Roboto)

  
| Column 1 | Column 2 | Column 3 | Column 4 |  
| --- | --- | --- | --- |  
| **Platform** | **Font family** | **Weight** | **Usage** |  
| **iOS** | San Francisco (SF) | Regular, Bold, Medium, Strong | Used across all text elements to ensure legibility |  
| **Android** | Roboto | Regular, Bold, Medium, Strong | Standard font for Android, optimized for multiple densities |  


System fonts are automatically optimized for each platform, reducing the need for manual adjustments across different screen sizes and resolutions.

---

# Space between text styles

To ensure visual balance, the following spacing rules must be applied depending on the typographic hierarchy:

  
| Column 1 | Column 2 | Column 3 |  
| --- | --- | --- |  
| **Text combination** | **Spacing (px)** | **Usage** |  
| **heading&hyphen;01 → subtitle** | 8px `stack&hyphen;sm`  | Between major headings and their subtitles |  
| **heading&hyphen;02 → subtitle** | 8px `stack&hyphen;sm`  | Between subheadings and their descriptors |  
| **title&hyphen;01 → subtitle** | 8px `stack&hyphen;sm`  | For sections with supporting descriptions |  
| **title&hyphen;02 → body&hyphen;03** | 8px `stack&hyphen;sm`  | Used between subsection titles and body text |  
| **body&hyphen;strong&hyphen;02 → caption&hyphen;01** | 8px `stack&hyphen;sm`  | Spacing between emphasized body text and its caption |  
| **body&hyphen;strong&hyphen;03 → caption** | 8px `stack&hyphen;sm`  | For minor text elements with slight emphasis |  
| **cta&hyphen;text&hyphen;link** | 8px `stack&hyphen;sm`  | Always placed with 16px spacing between body content and the CTA link |  


  
![DO space title ](https://studio-assets.supernova.io/design-systems/161625/f33d2b82-9327-4478-b941-1bcdf0af0829.png)  
DO space title   


> undefined  
> **Rules for proper hierarchy**:

1. **For major titles** (`heading&hyphen;01`, `heading&hyphen;02`, `title&hyphen;01`): Use `subtitle` or smaller for text immediately following the title.
2. **For mid&hyphen;level titles** (`title&hyphen;02`, `subtitle`): Use `body&hyphen;03` or smaller for text directly below.
3. **For lower&hyphen;level titles** (`body&hyphen;strong&hyphen;02`, `body&hyphen;strong&hyphen;03`): Use `caption` or smaller for any subsequent text.

---

# **Accessibility considerations**

Text contrast is crucial to ensure that typography is legible across various background surfaces. These rules define how text should contrast against different backgrounds, ensuring accessibility compliance across all apps.

- **Normal text (e.g., body text, captions)**: Minimum contrast ratio of **4.5:1**

- **Large text (e.g., headings, titles)**: Minimum contrast ratio of **3:1**

- **CTA links**: Minimum contrast ratio of **4.5:1**

The following table summarizes the required text color based on the background surface:

  
| Column 1 | Column 2 | Column 3 |  
| --- | --- | --- |  
| **Background** | **Minimum text color** | **Explanation** |  
| **surface** | **on&hyphen;surface&hyphen;low** | Use this for standard page backgrounds. |  
| **surface&hyphen;container&hyphen;low** | **on&hyphen;surface&hyphen;low** | For light containers, apply “on&hyphen;surface&hyphen;low” for smaller components or cards. |  
| **surface&hyphen;container&hyphen;mid** | **on&hyphen;surface&hyphen;mid** | For medium containers, apply “on&hyphen;surface&hyphen;mid” to ensure better contrast. |  
| **surface&hyphen;container&hyphen;high** | **on&hyphen;surface&hyphen;high** | For dark containers, apply “on&hyphen;surface&hyphen;high” for maximum readability. |  


  
![DO hierarchy typo](https://studio-assets.supernova.io/design-systems/161625/46f5fb8f-70e6-4295-a534-9f77c69b8075.png)  
DO hierarchy typo  


> undefined  
> **Specific contrast rules**

• **If the background is “surface”** (e.g., main page background): Text color must be **equal to or higher than “on&hyphen;surface&hyphen;low”**.
• **Component Backgrounds**:
• **“surface&hyphen;container&hyphen;low”**: Use **text color equal to or higher than “on&hyphen;surface&hyphen;low”**.
• **“surface&hyphen;container&hyphen;mid”**: Use **text color equal to or higher than “on&hyphen;surface&hyphen;mid”**.
• **“surface&hyphen;container&hyphen;high”**: Use **text color equal to or higher than “on&hyphen;surface&hyphen;high”**.

---

# Typescale

The following table presents the primary typography properties across both platforms of the app:

  
**🍏 iOS**  
  
  
fontWeight: 700px  
fontSize: 34px  
letterSpacing: 0px  
lineHeight: 41px  
  
  
  
fontWeight: 700px  
fontSize: 28px  
letterSpacing: 0px  
lineHeight: 34px  
  
  
  
fontWeight: 700px  
fontSize: 24px  
letterSpacing: 0px  
lineHeight: 28px  
  
  
  
fontWeight: 700px  
fontSize: 20px  
letterSpacing: 0px  
lineHeight: 24px  
  
  
  
fontWeight: 500px  
fontSize: 17px  
letterSpacing: -0.4099999964237213px  
lineHeight: 22px  
  
  
  
fontWeight: 400px  
fontSize: 17px  
letterSpacing: -0.4099999964237213px  
lineHeight: 22px  
  
  
  
fontWeight: 500px  
fontSize: 16px  
letterSpacing: 0px  
lineHeight: 16px  
  
  
  
fontWeight: 400px  
fontSize: 15px  
letterSpacing: 0px  
lineHeight: 20px  
  
  
  
fontWeight: 500px  
fontSize: 15px  
letterSpacing: 0px  
lineHeight: 20px  
  
  
  
fontWeight: 400px  
fontSize: 13px  
letterSpacing: 0px  
lineHeight: 18px  
  
  
  
fontWeight: 500px  
fontSize: 13px  
letterSpacing: 0px  
lineHeight: 18px  
  
  
  
fontWeight: 400px  
fontSize: 12px  
letterSpacing: 0px  
lineHeight: 16px  
  
  
  
fontWeight: 700px  
fontSize: 12px  
letterSpacing: 0px  
lineHeight: 16px  
  
  
  
fontWeight: 500px  
fontSize: 11px  
letterSpacing: 0px  
lineHeight: 13px  
  
  
  
fontWeight: 500px  
fontSize: 14px  
letterSpacing: 0px  
lineHeight: 14px  
  
  
**🤖 Android**  
  
  
fontWeight: 700px  
fontSize: 34px  
letterSpacing: 0.25px  
lineHeight: 40px  
  
  
  
fontWeight: 700px  
fontSize: 28px  
letterSpacing: 0px  
lineHeight: 32px  
  
  
  
fontWeight: 600px  
fontSize: 24px  
letterSpacing: 0.1500000059604645px  
lineHeight: 28px  
  
  
  
fontWeight: 600px  
fontSize: 20px  
letterSpacing: 0.1500000059604645px  
lineHeight: 24px  
  
  
  
fontWeight: 500px  
fontSize: 17px  
letterSpacing: 0.1500000059604645px  
lineHeight: 24px  
  
  
  
fontWeight: 400px  
fontSize: 17px  
letterSpacing: 0px  
lineHeight: 24px  
  
  
  
fontWeight: 500px  
fontSize: 16px  
letterSpacing: 0.75px  
lineHeight: 16px  
  
  
  
fontWeight: 400px  
fontSize: 14px  
letterSpacing: 0.25px  
lineHeight: 20px  
  
  
  
fontWeight: 500px  
fontSize: 14px  
letterSpacing: 0.1000000014901161px  
lineHeight: 20px  
  
  
  
fontWeight: 400px  
fontSize: 13px  
letterSpacing: 0.25px  
lineHeight: 18px  
  
  
  
fontWeight: 500px  
fontSize: 13px  
letterSpacing: 0px  
lineHeight: 18px  
  
  
  
fontWeight: 400px  
fontSize: 12px  
letterSpacing: 0.4000000059604645px  
lineHeight: 16px  
  
  
  
fontWeight: 500px  
fontSize: 12px  
letterSpacing: 0.4000000059604645px  
lineHeight: 16px  
  
  
  
fontWeight: 500px  
fontSize: 11px  
letterSpacing: 0.4000000059604645px  
lineHeight: 16px  
  
  
  
fontWeight: 500px  
fontSize: 14px  
letterSpacing: 0.1000000014901161px  
lineHeight: 20px  
  
