{
  "title": "💠 aem.card-image-default-container-v3",
  "anatomy": {
    "root": {
      "type": "container"
    },
    "wrapper": {
      "type": "container"
    },
    "display-options": {
      "type": "container"
    },
    "webtabs": {
      "type": "instance",
      "instanceOf": "webtabs"
    },
    "webcarousel": {
      "type": "container"
    },
    "items": {
      "type": "container"
    },
    "item-3": {
      "type": "instance",
      "instanceOf": "card-image-default-v3"
    },
    "item-1": {
      "type": "instance",
      "instanceOf": "card-image-default-v3"
    },
    "item-2": {
      "type": "instance",
      "instanceOf": "card-image-default-v3"
    },
    "webpagination-condensed": {
      "type": "instance",
      "instanceOf": "webpagination-condensed"
    }
  },
  "props": {
    "display-options": {
      "type": "boolean",
      "default": true
    },
    "": {
      "type": "string",
      "default": "1+",
      "enum": [
        "1",
        "1+",
        "2",
        "2+",
        "3",
        "3+",
        "4",
        "4+",
        "5",
        "5+"
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
    },
    "display": {
      "type": "string",
      "default": "carousel",
      "enum": [
        "grid",
        "carousel"
      ]
    }
  },
  "default": {
    "name": "# columns on desktop-md=1, # items=1+, breakpoint=desktop-md (1280-1439), display=carousel",
    "elements": {
      "root": {
        "children": [
          "wrapper"
        ],
        "styles": {
          "width": 1340,
          "counterAxisAlignItems": "CENTER",
          "layoutMode": "VERTICAL",
          "itemSpacing": "breakpoints/wel/sem/spacingDynamic/withinSection/2xl",
          "paddingLeft": "breakpoints/wel/sem/sizing/grid/margins",
          "paddingRight": "breakpoints/wel/sem/sizing/grid/margins"
        }
      },
      "wrapper": {
        "parent": "root",
        "children": [
          "display-options",
          "webcarousel"
        ],
        "styles": {
          "layoutMode": "VERTICAL",
          "layoutSizingHorizontal": "FILL",
          "layoutSizingVertical": "HUG",
          "itemSpacing": "breakpoints/wel/sem/spacingStatic/stack/lg"
        }
      },
      "display-options": {
        "parent": "wrapper",
        "children": [
          "webtabs"
        ],
        "styles": {
          "primaryAxisAlignItems": "MAX",
          "counterAxisAlignItems": "CENTER",
          "layoutMode": "HORIZONTAL",
          "layoutSizingHorizontal": "FILL",
          "layoutSizingVertical": "HUG",
          "itemSpacing": "breakpoints/wel/sem/spacingStatic/inline/xl"
        },
        "propReferences": {
          "visible": {
            "$ref": "#/props/display-options"
          }
        }
      },
      "webtabs": {
        "parent": "display-options",
        "styles": {
          "layoutSizingHorizontal": "FILL",
          "layoutSizingVertical": "HUG"
        },
        "propConfigurations": {
          "tabs": "1745255441",
          "left-button": "false",
          "more-tabs": "false",
          "truncation": "false",
          "right-button": "true",
          "align": "flex-start",
          "display": "inline"
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
          "item-3",
          "item-1",
          "item-2"
        ],
        "styles": {
          "primaryAxisAlignItems": "CENTER",
          "layoutMode": "HORIZONTAL",
          "layoutSizingHorizontal": "FILL",
          "layoutSizingVertical": "HUG",
          "itemSpacing": "breakpoints/wel/sem/spacingDynamic/inline/xl"
        }
      },
      "item-3": {
        "parent": "items",
        "styles": {
          "layoutSizingVertical": "HUG",
          "width": 1212
        },
        "propConfigurations": {
          "focus": "false",
          "breakpoint": "desktop-md-1280-1439"
        }
      },
      "item-1": {
        "parent": "items",
        "styles": {
          "layoutSizingVertical": "HUG",
          "width": 1212
        },
        "propConfigurations": {
          "focus": "false",
          "breakpoint": "desktop-md-1280-1439"
        }
      },
      "item-2": {
        "parent": "items",
        "styles": {
          "layoutSizingVertical": "HUG",
          "width": 1212
        },
        "propConfigurations": {
          "focus": "false",
          "breakpoint": "desktop-md-1280-1439"
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
          "step": "1-3",
          "size": "md",
          "align": "right",
          "loop": "false"
        }
      }
    }
  },
  "variants": [
    {
      "name": "# columns on desktop-md=1, # items=1+, breakpoint=desktop-md (1280-1439), display=grid",
      "configuration": {
        "display": "grid"
      },
      "elements": {
        "root": {
          "styles": {
            "counterAxisAlignItems": "MIN"
          }
        },
        "wrapper": {
          "children": [
            "display-options",
            "items"
          ]
        },
        "webtabs": {
          "propConfigurations": {
            "left-button": "false",
            "more-tabs": "false",
            "truncation": "true",
            "right-button": "true"
          }
        },
        "items": {
          "parent": "wrapper",
          "children": [
            "item-1",
            "item-2"
          ],
          "styles": {
            "primaryAxisAlignItems": "MIN",
            "layoutMode": "VERTICAL"
          }
        },
        "item-1": {
          "styles": {
            "layoutSizingHorizontal": "FILL"
          },
          "propConfigurations": {
            "focus": "false"
          }
        },
        "item-2": {
          "styles": {
            "layoutSizingHorizontal": "FILL"
          },
          "propConfigurations": {
            "focus": "false"
          }
        },
        "item-3": {
          "propConfigurations": {
            "focus": "false"
          }
        }
      }
    },
    {
      "name": "# columns on desktop-md=1, # items=1+, breakpoint=tablet (768-1023), display=carousel",
      "configuration": {
        "breakpoint": "tablet (768-1023)"
      },
      "elements": {
        "root": {
          "styles": {
            "width": 768,
            "counterAxisAlignItems": "MIN"
          }
        },
        "webtabs": {
          "propConfigurations": {
            "left-button": "false",
            "more-tabs": "false",
            "truncation": "false"
          }
        },
        "item-3": {
          "propConfigurations": {
            "focus": "false"
          }
        },
        "item-1": {
          "propConfigurations": {
            "focus": "false"
          }
        },
        "item-2": {
          "propConfigurations": {
            "focus": "false"
          }
        }
      }
    },
    {
      "name": "# columns on desktop-md=1, # items=1+, breakpoint=desktop-sm (1024-1279), display=carousel",
      "configuration": {
        "breakpoint": "desktop-sm (1024-1279)"
      },
      "elements": {
        "root": {
          "styles": {
            "width": 1024,
            "counterAxisAlignItems": "MIN"
          }
        },
        "webtabs": {
          "propConfigurations": {
            "left-button": "false",
            "more-tabs": "false",
            "truncation": "false"
          }
        },
        "item-3": {
          "propConfigurations": {
            "focus": "false"
          }
        },
        "item-1": {
          "propConfigurations": {
            "focus": "false"
          }
        },
        "item-2": {
          "propConfigurations": {
            "focus": "false"
          }
        }
      }
    },
    {
      "name": "# columns on desktop-md=1, # items=1, breakpoint=desktop-md (1280-1439), display=carousel",
      "configuration": {
        "# items": "1"
      },
      "elements": {
        "root": {
          "styles": {
            "counterAxisAlignItems": "MIN"
          }
        },
        "wrapper": {
          "children": [
            "display-options",
            "items"
          ]
        },
        "webtabs": {
          "propConfigurations": {
            "left-button": "false",
            "more-tabs": "false",
            "truncation": "false"
          }
        },
        "items": {
          "parent": "wrapper",
          "children": [
            "item-1"
          ]
        },
        "item-1": {
          "styles": {
            "layoutSizingHorizontal": "FILL"
          },
          "propConfigurations": {
            "focus": "false"
          }
        },
        "item-3": {
          "propConfigurations": {
            "focus": "false"
          }
        },
        "item-2": {
          "propConfigurations": {
            "focus": "false"
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
      "# items": "2"
    },
    {
      "# items": "2+"
    },
    {
      "# items": "3"
    },
    {
      "# items": "3+"
    },
    {
      "# items": "4"
    },
    {
      "# items": "4+"
    },
    {
      "# items": "5"
    },
    {
      "# items": "5+"
    },
    {
      "# columns on desktop-md": "2"
    },
    {
      "# columns on desktop-md": "3"
    },
    {
      "# columns on desktop-md": "4"
    },
    {
      "# columns on desktop-md": "5"
    }
  ],
  "metadata": {
    "author": "Arthur MATHON",
    "lastUpdated": "2025-12-04T16:44:03.261Z",
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
      "nodeId": "7846:155492"
    }
  }
}