
# Recurrent properties

---

> Be warned:  
> In practice, it can be challenging to decide whether elements below should be named a variant or a property. As a rule of thumb, the more change involved when switching between values, the more it makes sense to treat it as a variant rather than a property.

  
| Column 1 | Column 2 |  
| --- | --- |  
| Property | Description |  
| size | The various dimensions of a component |  
| :state | The various component states |  
| breakpoint | The Variations of a component based on the viewport’s size (not the container’s). |  
| content | Controls the sub&hyphen;elements of a component |  
| emphasis | The hierarchical level within a given function or variation |  
| function | The semantic function paired with a given UI element (for instance: Message) |  
| quantity | The number of sub&hyphen;elements |  
| type | A semantic definition that's neither a function nor a content |  


If you want to learn more about usual values and how to actually name things in various platforms, head over to the [Property naming](../property-naming.md) page of this section.

> Some extra info:  
> In the app, the 'breakpoint' property is renamed 'screen size' to align with the OS viewport specifications. Additionally, it's sometimes necessary to specify the operating system in the properties using the 'platform' attribute.

  
| Column 1 | Column 2 |  
| --- | --- |  
| Property | Description |  
| ~~Breakpoint~~ Screen size | Variations of a component align with the OS viewport specifications.  |  
| Platform | ‘iOS’ or ‘Android’ |  
