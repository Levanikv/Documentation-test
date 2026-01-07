
# Example

---

Imagine a Product Designer needs the [**Badge**](#)** **component to show a Tooltip on hover, providing users with more information about its content.

# Design need

  
![Update](https://studio-assets.supernova.io/design-systems/161625/3fba6803-c193-4cce-a1cb-4189fce464e4.png)  
Update  


The first step is usually a Figma mockup of the update, created directly in the contributor’s working file (Discovery files).

# Design System review

  
![Review](https://studio-assets.supernova.io/design-systems/161625/59246f5e-a6b1-4ebe-ada1-c97ec8f97cef.png)  
Review  


Next, a Design System Manager (DSM) meets with the Product Designer to review the submission. During this meeting, DSMs check if:

- The proposal complies with Welcome’s design principles.

- Welcome’s Foundations are used (or can be used to achieve the same visual result).

- No other component in the Design System can achieve the same outcome.

- The component or update is likely to be accessible (with support from an accessibility expert if needed).

- The contribution meets the [inclusion criteria](./presentation.md).

# Move to Candidate

In this example, almost all inclusion criteria are met:

- **Stable ✅ **: The designer is confident in the design and ready to deliver.

- **Agnostic ✅ **: The update has no business&hyphen; or context&hyphen;specific aspects.

- **Simple ✅ **: The update is easy to implement.

- **Common ✅ **: Such behavior is not uncommon, similar to [Carbon’s Tag](https://carbondesignsystem.com/components/tag/usage/#operational-tag) component.

- **Reusable ❌ **: This criterion is not yet met, so a public consultation will be held to confirm reuse.

In the meantime, the DSM and Product Designer can refine the design and move it to the Candidate library. A JIRA ticket is created in the Design System team’s backlog to track progress. Automated subtasks cover every contribution step (Design, Specifications, Documentation).

  
![Ticket](https://studio-assets.supernova.io/design-systems/161625/8e91d2b3-cd4b-46ef-b307-7056b810414b.png)  
Ticket  


# Public poll

A public poll is held in the “Design System Requests” Teams channel. This quick poll confirms traction and potential reuse among designers.

  
![Poll](https://studio-assets.supernova.io/design-systems/161625/10d7f5c7-c251-45ec-a7eb-8ee5aa0a93a1.png)  
Poll  


If a majority agrees, all criteria are met, and the update can proceed to the Core Team or the Feature Team that needs it.

# Specifications

During or after the poll, the DSM writes the component’s specifications on a hidden page in Supernova. This page includes all details typically found in component documentation.

  
![Specs](https://studio-assets.supernova.io/design-systems/161625/fd62152b-245a-4c85-808c-2b1004483653.png)  
Specs  


# Implementation

After specifications are complete, they’re passed to the development team via a dedicated JIRA ticket linked to the original Design System ticket. Once prioritized, the update is included in an upcoming sprint for development and release.