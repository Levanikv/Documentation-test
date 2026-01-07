{

&nbsp; "title": "💠 aem.card-image-wide-container-v3",

&nbsp; "anatomy": {

&nbsp;   "root": {

&nbsp;     "type": "container"

&nbsp;   },

&nbsp;   "wrapper": {

&nbsp;     "type": "container"

&nbsp;   },

&nbsp;   "display-options": {

&nbsp;     "type": "container"

&nbsp;   },

&nbsp;   "webtabs": {

&nbsp;     "type": "instance",

&nbsp;     "instanceOf": "webtabs"

&nbsp;   },

&nbsp;   "items": {

&nbsp;     "type": "container"

&nbsp;   },

&nbsp;   "card-image-wide-v3": {

&nbsp;     "type": "instance",

&nbsp;     "instanceOf": "card-image-wide-v3"

&nbsp;   },

&nbsp;   "webcarousel": {

&nbsp;     "type": "instance",

&nbsp;     "detectedIn": "# items=2+, breakpoint=desktop-md (1280-1439)",

&nbsp;     "instanceOf": "webcarousel"

&nbsp;   }

&nbsp; },

&nbsp; "props": {

&nbsp;   "display-options": {

&nbsp;     "type": "boolean",

&nbsp;     "default": true

&nbsp;   },

&nbsp;   "": {

&nbsp;     "type": "string",

&nbsp;     "default": "1",

&nbsp;     "enum": \[

&nbsp;       "1",

&nbsp;       "2+"

&nbsp;     ]

&nbsp;   },

&nbsp;   "breakpoint": {

&nbsp;     "type": "string",

&nbsp;     "default": "desktop-md (1280-1439)",

&nbsp;     "enum": \[

&nbsp;       "mobile (320-767)",

&nbsp;       "tablet (768-1023)",

&nbsp;       "desktop-sm (1024-1279)",

&nbsp;       "desktop-md (1280-1439)"

&nbsp;     ]

&nbsp;   }

&nbsp; },

&nbsp; "default": {

&nbsp;   "name": "# items=1, breakpoint=desktop-md (1280-1439)",

&nbsp;   "elements": {

&nbsp;     "root": {

&nbsp;       "children": \[

&nbsp;         "wrapper"

&nbsp;       ],

&nbsp;       "styles": {

&nbsp;         "width": 1340,

&nbsp;         "layoutMode": "VERTICAL",

&nbsp;         "itemSpacing": "breakpoints/wel/sem/spacingDynamic/withinSection/2xl",

&nbsp;         "paddingLeft": "breakpoints/wel/sem/sizing/grid/margins",

&nbsp;         "paddingRight": "breakpoints/wel/sem/sizing/grid/margins"

&nbsp;       }

&nbsp;     },

&nbsp;     "wrapper": {

&nbsp;       "parent": "root",

&nbsp;       "children": \[

&nbsp;         "display-options",

&nbsp;         "items"

&nbsp;       ],

&nbsp;       "styles": {

&nbsp;         "layoutMode": "VERTICAL",

&nbsp;         "layoutSizingHorizontal": "FILL",

&nbsp;         "layoutSizingVertical": "HUG",

&nbsp;         "itemSpacing": "breakpoints/wel/sem/spacingStatic/stack/lg"

&nbsp;       }

&nbsp;     },

&nbsp;     "display-options": {

&nbsp;       "parent": "wrapper",

&nbsp;       "children": \[

&nbsp;         "webtabs"

&nbsp;       ],

&nbsp;       "styles": {

&nbsp;         "primaryAxisAlignItems": "MAX",

&nbsp;         "counterAxisAlignItems": "CENTER",

&nbsp;         "layoutMode": "HORIZONTAL",

&nbsp;         "layoutSizingHorizontal": "FILL",

&nbsp;         "layoutSizingVertical": "HUG",

&nbsp;         "itemSpacing": "breakpoints/wel/sem/spacingStatic/inline/xl"

&nbsp;       },

&nbsp;       "propReferences": {

&nbsp;         "visible": {

&nbsp;           "$ref": "#/props/display-options"

&nbsp;         }

&nbsp;       }

&nbsp;     },

&nbsp;     "webtabs": {

&nbsp;       "parent": "display-options",

&nbsp;       "styles": {

&nbsp;         "layoutSizingHorizontal": "FILL",

&nbsp;         "layoutSizingVertical": "HUG"

&nbsp;       },

&nbsp;       "propConfigurations": {

&nbsp;         "tabs": "1745255441",

&nbsp;         "left-button": "false",

&nbsp;         "more-tabs": "false",

&nbsp;         "truncation": "false",

&nbsp;         "right-button": "true",

&nbsp;         "align": "flex-start",

&nbsp;         "display": "inline"

&nbsp;       }

&nbsp;     },

&nbsp;     "items": {

&nbsp;       "parent": "wrapper",

&nbsp;       "children": \[

&nbsp;         "card-image-wide-v3"

&nbsp;       ],

&nbsp;       "styles": {

&nbsp;         "primaryAxisAlignItems": "CENTER",

&nbsp;         "layoutMode": "HORIZONTAL",

&nbsp;         "layoutSizingHorizontal": "FILL",

&nbsp;         "layoutSizingVertical": "HUG",

&nbsp;         "itemSpacing": "breakpoints/wel/sem/spacingDynamic/inline/xl"

&nbsp;       }

&nbsp;     },

&nbsp;     "card-image-wide-v3": {

&nbsp;       "parent": "items",

&nbsp;       "styles": {

&nbsp;         "layoutSizingHorizontal": "FILL",

&nbsp;         "layoutSizingVertical": "HUG"

&nbsp;       },

&nbsp;       "propConfigurations": {

&nbsp;         "breakpoint": "desktop-md-1280-1439",

&nbsp;         "content-alignment": "right"

&nbsp;       }

&nbsp;     },

&nbsp;     "webcarousel": {

&nbsp;       "styles": {

&nbsp;         "layoutSizingHorizontal": "FILL",

&nbsp;         "layoutSizingVertical": "HUG"

&nbsp;       },

&nbsp;       "propConfigurations": {

&nbsp;         "gradient-mask": "true",

&nbsp;         "breakpoint": "desktop-md-1280-1439",

&nbsp;         "": "1",

&nbsp;         "align": "left",

&nbsp;         "display": "full-grid",

&nbsp;         "scroll": "start"

&nbsp;       }

&nbsp;     }

&nbsp;   }

&nbsp; },

&nbsp; "variants": \[

&nbsp;   {

&nbsp;     "name": "# items=1, breakpoint=mobile (320-767)",

&nbsp;     "configuration": {

&nbsp;       "breakpoint": "mobile (320-767)"

&nbsp;     },

&nbsp;     "elements": {

&nbsp;       "root": {

&nbsp;         "styles": {

&nbsp;           "width": 375

&nbsp;         }

&nbsp;       },

&nbsp;       "webtabs": {

&nbsp;         "propConfigurations": {

&nbsp;           "left-button": "false",

&nbsp;           "more-tabs": "false",

&nbsp;           "truncation": "false"

&nbsp;         }

&nbsp;       },

&nbsp;       "card-image-wide-v3": {

&nbsp;         "propConfigurations": {

&nbsp;           "breakpoint": "mobile-320-767",

&nbsp;           "content-alignment": "bottom"

&nbsp;         }

&nbsp;       }

&nbsp;     }

&nbsp;   },

&nbsp;   {

&nbsp;     "name": "# items=1, breakpoint=tablet (768-1023)",

&nbsp;     "configuration": {

&nbsp;       "breakpoint": "tablet (768-1023)"

&nbsp;     },

&nbsp;     "elements": {

&nbsp;       "root": {

&nbsp;         "styles": {

&nbsp;           "width": 768

&nbsp;         }

&nbsp;       },

&nbsp;       "webtabs": {

&nbsp;         "propConfigurations": {

&nbsp;           "left-button": "false",

&nbsp;           "more-tabs": "false",

&nbsp;           "truncation": "false"

&nbsp;         }

&nbsp;       },

&nbsp;       "card-image-wide-v3": {

&nbsp;         "propConfigurations": {

&nbsp;           "breakpoint": "tablet-768-1023"

&nbsp;         }

&nbsp;       }

&nbsp;     }

&nbsp;   },

&nbsp;   {

&nbsp;     "name": "# items=1, breakpoint=desktop-sm (1024-1279)",

&nbsp;     "configuration": {

&nbsp;       "breakpoint": "desktop-sm (1024-1279)"

&nbsp;     },

&nbsp;     "elements": {

&nbsp;       "root": {

&nbsp;         "styles": {

&nbsp;           "width": 1024

&nbsp;         }

&nbsp;       },

&nbsp;       "webtabs": {

&nbsp;         "propConfigurations": {

&nbsp;           "left-button": "false",

&nbsp;           "more-tabs": "false",

&nbsp;           "truncation": "false"

&nbsp;         }

&nbsp;       },

&nbsp;       "card-image-wide-v3": {

&nbsp;         "propConfigurations": {

&nbsp;           "breakpoint": "desktop-sm-1024-1279"

&nbsp;         }

&nbsp;       }

&nbsp;     }

&nbsp;   },

&nbsp;   {

&nbsp;     "name": "# items=2+, breakpoint=desktop-md (1280-1439)",

&nbsp;     "configuration": {

&nbsp;       "# items": "2+"

&nbsp;     },

&nbsp;     "elements": {

&nbsp;       "wrapper": {

&nbsp;         "children": \[

&nbsp;           "display-options",

&nbsp;           "webcarousel"

&nbsp;         ],

&nbsp;         "styles": {

&nbsp;           "layoutSizingHorizontal": "FIXED",

&nbsp;           "width": 1212

&nbsp;         }

&nbsp;       },

&nbsp;       "webtabs": {

&nbsp;         "propConfigurations": {

&nbsp;           "left-button": "false",

&nbsp;           "more-tabs": "false",

&nbsp;           "truncation": "false"

&nbsp;         }

&nbsp;       },

&nbsp;       "webcarousel": {

&nbsp;         "parent": "wrapper"

&nbsp;       }

&nbsp;     }

&nbsp;   }

&nbsp; ],

&nbsp; "invalidVariantCombinations": \[],

&nbsp; "metadata": {

&nbsp;   "author": "Arthur MATHON",

&nbsp;   "lastUpdated": "2025-12-04T16:23:52.722Z",

&nbsp;   "generator": {

&nbsp;     "url": "https://www.figma.com/community/plugin/1549454283615386215/anova",

&nbsp;     "version": 4,

&nbsp;     "name": "Directed Edges Anova Figma Plugin"

&nbsp;   },

&nbsp;   "schema": {

&nbsp;     "url": "https://github.com/DirectedEdges/anova/blob/main/anova.schema.json",

&nbsp;     "version": "0.3.0"

&nbsp;   },

&nbsp;   "source": {

&nbsp;     "pageId": "5735:27578",

&nbsp;     "nodeId": "7868:49223"

&nbsp;   }

&nbsp; }

}

