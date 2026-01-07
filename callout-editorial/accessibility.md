
# Accessibility

---

# Accessibility

Callout Editorial follows WCAG 2.2 Level AA standards to ensure an inclusive experience for all users across different devices and assistive technologies.

# WCAG 2.2

  
**Keyboard navigation**  
✅ Users can navigate through all interactive elements within Callout Editorial using keyboard controls, meeting [2.1.1 Keyboard (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/keyboard.html) and [2.1.3 Keyboard (No Exception) (Level AAA)](https://www.w3.org/WAI/WCAG22/Understanding/keyboard-no-exception.html).&ast;
**Navigation sequence:**  
- Use `TAB` to move forward through interactive elements in this order: Media (if linked), Logo Slot, Badges, title (if linked), USP section, and call&hyphen;to&hyphen;action Button.  
- Use `SHIFT+TAB` to move backward through interactive elements.  
- Use `ENTER` or `SPACE` to activate Buttons and select options.  
**Focus indicators:** All interactive elements display a visible focus indicator that meets [2.4.7 Focus Visible (Level AA)](https://www.w3.org/WAI/WCAG22/Understanding/focus-visible.html) and [2.4.11 Focus Not Obscured (Minimum) (Level AA)](https://www.w3.org/WAI/WCAG22/Understanding/focus-not-obscured-minimum.html). Focus states use the `focus` color token to ensure consistent visibility across different background surfaces, achieving the 3:1 contrast requirement specified in [1.4.11 Non&hyphen;text Contrast (Level AA)](https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast.html). The focus order follows a logical sequence as required by [2.4.3 Focus Order (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/focus-order.html).  
  
**Screen reader support**  
✅ Callout Editorial Container provides appropriate semantic structure and labels for screen reader users, conforming to [4.1.2 Name, Role, Value (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html).
  
**Landmark regions:**  
- The component uses appropriate ARIA landmarks to help users understand the content structure, supporting [1.3.1 Info and Relationships (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/info-and-relationships.html).  
- The image area (Media instance) includes proper role attributes and alternative text.  
- Badge groups are announced as related items for context.  
**Announcements:**  
- When users interact with the call&hyphen;to&hyphen;action button, screen readers announce the action and destination, meeting [4.1.3 Status Messages (Level AA)](https://www.w3.org/WAI/WCAG22/Understanding/status-messages.html).  
- Kicker text provides contextual information announced before the title.  
- Badge content is announced with appropriate labels indicating their function (family&hyphen;friendly, offer, default).  
**Labels:**  
- The title element provides the primary accessible name for the callout.  
- Each Badge maintains its own accessible name and role.  
- The call&hyphen;to&hyphen;action (Button) includes accessible labels indicating the action.  
  
**Interactive elements**  
✅ All interactive elements meet the minimum touch target size of 44×44 pixels on mobile devices, exceeding the requirements of [2.5.5 Target Size (Enhanced) (Level AAA)](https://www.w3.org/WAI/WCAG22/Understanding/target-size-enhanced.html) and conforming to [2.5.8 Target Size (Minimum) (Level AA)](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html).  

**Button states:** ✅ Interactive elements provide clear visual and programmatic states that meet [3.2.4 Consistent Identification (Level AA)](https://www.w3.org/WAI/WCAG22/Understanding/consistent-identification.html):  
- Default state with sufficient contrast  
- Hover state for pointer devices  
- Focus state for keyboard navigation  
- Pressed state for active interaction  
- Disabled state when actions are unavailable (shown at 38% opacity)  
All state changes are perceivable through multiple visual cues, not relying solely on color to convey information, as required by [1.4.1 Use of Color (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/use-of-color.html).  
  
**Color contrast**  
✅ Callout Editorial maintains sufficient color contrast across both background variants:  
- **Background: no** – Text colors (`on&hyphen;surface&hyphen;hi`, `on&hyphen;surface&hyphen;mid`, `on&hyphen;surface&hyphen;low`) provide adequate contrast against the transparent background, meeting [1.4.3 Contrast (Minimum) (Level AA)](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html).  
- **Background: yes** – The `surface&hyphen;container&hyphen;low` background in the bottom section ensures text remains readable with proper contrast ratios.  


# Best practices

**Content considerations:**

- Ensure the title text is descriptive and meaningful, satisfying [2.4.4 Link Purpose (In Context) (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/link-purpose-in-context.html) when Callout is interactive.

- Provide meaningful alternative text for the image that describes its content or purpose, supporting [1.1.1 Non&hyphen;text Content (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/non-text-content.html).

- Use Kicker to provide additional context that helps users understand Callout's purpose.

- Limit the number of Badges to prevent cognitive overload, aligning with accessibility best practices.

**Implementation guidelines:**

- Always provide text alternatives for any visual&hyphen;only information, meeting [1.1.1 Non&hyphen;text Content (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/non-text-content.html).

- Ensure Button has a clear, descriptive label per [2.1.1 Keyboard (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/keyboard.html).

- When using Logo Slot, ensure the logo has appropriate alternative text or is marked as decorative.

- Verify that the USP section (icon and label) conveys meaning through text, not icon alone.

**Testing recommendations:**

- Test with keyboard&hyphen;only navigation to verify all functionality is accessible per [2.1.1 Keyboard (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/keyboard.html).

- Use screen readers (NVDA, JAWS, VoiceOver) to validate announcements and structure against [4.1.2 Name, Role, Value (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html).

- Check color contrast in both background variants using tools that verify [1.4.3 Contrast (Minimum) (Level AA)](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html) and [1.4.11 Non&hyphen;text Contrast (Level AA)](https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast.html).

- Verify touch target sizes on actual mobile devices per [2.5.8 Target Size (Minimum) (Level AA)](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html).

- Test with browser zoom at 200% to ensure content remains accessible and usable, meeting [1.4.4 Resize Text (Level AA)](https://www.w3.org/WAI/WCAG22/Understanding/resize-text.html) and [1.4.10 Reflow (Level AA)](https://www.w3.org/WAI/WCAG22/Understanding/reflow.html).
