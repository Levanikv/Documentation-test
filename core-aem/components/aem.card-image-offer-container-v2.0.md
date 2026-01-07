{
  "title": "💠 aem.card-image-offer-container-v1",
  "anatomy": {
    "root": {
      "type": "container"
    },
    "wrapper": {
      "type": "container"
    },
    "webcarousel": {
      "type": "container"
    },
    "items": {
      "type": "container"
    },
    "item-5": {
      "type": "instance",
      "instanceOf": "card-image-offer-v1"
    },
    "item-1": {
      "type": "instance",
      "instanceOf": "card-image-offer-v1"
    },
    "item-2": {
      "type": "instance",
      "instanceOf": "card-image-offer-v1"
    },
    "item-3": {
      "type": "instance",
      "instanceOf": "card-image-offer-v1"
    },
    "item-4": {
      "type": "instance",
      "instanceOf": "card-image-offer-v1"
    },
    "webpagination-condensed": {
      "type": "instance",
      "instanceOf": "webpagination-condensed"
    }
  },
  "props": {
    "": {
      "type": "string",
      "default": "3+",
      "enum": [
        "1",
        "2",
        "3",
        "3+"
      ]
    },
    "breakpoint": {
      "type": "string",
      "default": "desktop-md (1280-1439)",
      "enum": [
        "mobile (320-767)",
        "tablet (768-1023)",
        "desktop-sm (1024-1279)",
        "desktop-md (1280-1439)"
      ]
    }
  },
  "default": {
    "name": "# columns on desktop-md=3, # items=3+, breakpoint=desktop-md (1280-1439)",
    "elements": {
      "root": {
        "children": [
          "wrapper"
        ],
        "styles": {
          "width": 1340,
          "layoutMode": "VERTICAL",
          "itemSpacing": "breakpoints/wel/sem/spacingDynamic/withinSection/2xl",
          "paddingLeft": "breakpoints/wel/sem/sizing/grid/margins",
          "paddingRight": "breakpoints/wel/sem/sizing/grid/margins"
        }
      },
      "wrapper": {
        "parent": "root",
        "children": [
          "webcarousel"
        ],
        "styles": {
          "layoutMode": "VERTICAL",
          "layoutSizingHorizontal": "FILL",
          "layoutSizingVertical": "HUG",
          "itemSpacing": "breakpoints/wel/sem/spacingStatic/stack/lg"
        }
      },
      "webcarousel": {
        "parent": "wrapper",
        "children": [
          "items",
          "webpagination-condensed"
        ],
        "styles": {
          "layoutMode": "VERTICAL",
          "layoutSizingHorizontal": "FILL",
          "layoutSizingVertical": "HUG",
          "itemSpacing": "breakpoints/wel/sem/spacingDynamic/stack/lg"
        }
      },
      "items": {
        "parent": "webcarousel",
        "children": [
          "item-5",
          "item-1",
          "item-2",
          "item-3",
          "item-4"
        ],
        "styles": {
          "primaryAxisAlignItems": "CENTER",
          "layoutMode": "HORIZONTAL",
          "layoutSizingHorizontal": "FILL",
          "layoutSizingVertical": "HUG",
          "itemSpacing": "breakpoints/wel/sem/spacingDynamic/inline/xl"
        }
      },
      "item-5": {
        "parent": "items",
        "styles": {
          "layoutSizingVertical": "HUG",
          "width": 388
        }
      },
      "item-1": {
        "parent": "items",
        "styles": {
          "layoutSizingVertical": "HUG",
          "width": 388
        }
      },
      "item-2": {
        "parent": "items",
        "styles": {
          "layoutSizingVertical": "HUG",
          "width": 388
        }
      },
      "item-3": {
        "parent": "items",
        "styles": {
          "layoutSizingVertical": "HUG",
          "width": 388
        }
      },
      "item-4": {
        "parent": "items",
        "styles": {
          "layoutSizingVertical": "HUG",
          "width": 388
        }
      },
      "webpagination-condensed": {
        "parent": "webcarousel",
        "styles": {
          "layoutSizingHorizontal": "FILL",
          "layoutSizingVertical": "HUG"
        },
        "propConfigurations": {
          "counter": "true",
          "step": "1-4",
          "size": "md",
          "align": "right",
          "loop": "false"
        }
      }
    }
  },
  "variants": [
    {
      "name": "# columns on desktop-md=3, # items=3+, breakpoint=desktop-sm (1024-1279)",
      "configuration": {
        "breakpoint": "desktop-sm (1024-1279)"
      },
      "elements": {
        "root": {
          "styles": {
            "width": 1024
          }
        }
      }
    },
    {
      "name": "# columns on desktop-md=3, # items=3, breakpoint=desktop-md (1280-1439)",
      "configuration": {
        "# items": "3"
      },
      "elements": {
        "wrapper": {
          "children": [
            "items"
          ]
        },
        "items": {
          "parent": "wrapper",
          "children": [
            "item-1",
            "item-2",
            "item-3"
          ]
        },
        "item-1": {
          "styles": {
            "layoutSizingHorizontal": "FILL"
          }
        },
        "item-2": {
          "styles": {
            "layoutSizingHorizontal": "FILL"
          }
        },
        "item-3": {
          "styles": {
            "layoutSizingHorizontal": "FILL"
          }
        }
      }
    }
  ],
  "invalidVariantCombinations": [
    {
      "breakpoint": "mobile (320-767)"
    },
    {
      "breakpoint": "tablet (768-1023)"
    },
    {
      "# items": "1"
    },
    {
      "# items": "2"
    },
    {
      "# columns on desktop-md": "1"
    },
    {
      "# columns on desktop-md": "2"
    }
  ],
  "metadata": {
    "author": "Arthur MATHON",
    "lastUpdated": "2025-12-04T16:10:50.225Z",
    "generator": {
      "url": "https://www.figma.com/community/plugin/1549454283615386215/anova",
      "version": 4,
      "name": "Directed Edges Anova Figma Plugin"
    },
    "schema": {
      "url": "https://github.com/DirectedEdges/anova/blob/main/anova.schema.json",
      "version": "0.3.0"
    },
    "source": {
      "pageId": "5735:27578",
      "nodeId": "7938:267855"
    }
  }
}