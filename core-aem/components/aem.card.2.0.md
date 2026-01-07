{
  "title": "💠 aem.card",
  "anatomy": {
    "root": {
      "type": "container"
    },
    "appendix": {
      "type": "instance",
      "instanceOf": "contentcardappendix"
    },
    "textsaction": {
      "type": "container"
    },
    "texts": {
      "type": "container"
    },
    "title": {
      "type": "text"
    },
    "subtitle": {
      "type": "text"
    },
    "description": {
      "type": "text"
    },
    "action": {
      "type": "instance",
      "instanceOf": "contentcardaction"
    }
  },
  "props": {
    "subtitle": {
      "type": "boolean",
      "default": true
    },
    "description": {
      "type": "boolean",
      "default": true
    },
    "action": {
      "type": "boolean",
      "default": true
    },
    "breakpoint": {
      "type": "string",
      "default": "mobile (320-767)",
      "enum": [
        "mobile (320-767)",
        "tablet (768-1023)",
        "desktop-sm (1024-1279)",
        "desktop-md (1280-1439)"
      ]
    },
    "appendix-left": {
      "type": "boolean",
      "default": true
    },
    "appendix-top": {
      "type": "boolean",
      "default": false
    }
  },
  "default": {
    "name": "breakpoint=mobile (320-767)",
    "elements": {
      "root": {
        "children": [
          "appendix",
          "textsaction"
        ],
        "styles": {
          "fills": "colorModes/wel/sem/color/surface-container-low",
          "cornerRadius": "breakpoints/wel/sem/borderRadius/surface",
          "width": 343,
          "layoutMode": "HORIZONTAL",
          "strokes": "colorModes/wel/sem/color/outline-low",
          "strokeWeight": "breakpoints/wel/sem/borderWidth/default",
          "itemSpacing": "breakpoints/wel/sem/spacingDynamic/inline/xl",
          "paddingLeft": "breakpoints/wel/sem/spacingDynamic/inset/xl",
          "paddingRight": "breakpoints/wel/sem/spacingDynamic/inset/xl",
          "paddingTop": "breakpoints/wel/sem/spacingDynamic/inset/xl",
          "paddingBottom": "breakpoints/wel/sem/spacingDynamic/inset/xl"
        }
      },
      "appendix": {
        "parent": "textsaction",
        "styles": {
          "visible": false,
          "width": 72,
          "height": 72
        },
        "propConfigurations": {
          "asset": "icon"
        },
        "propReferences": {
          "visible": {
            "$ref": "#/props/appendix top"
          }
        }
      },
      "textsaction": {
        "parent": "root",
        "children": [
          "appendix",
          "texts",
          "action"
        ],
        "styles": {
          "layoutMode": "VERTICAL",
          "layoutSizingHorizontal": "FILL",
          "layoutSizingVertical": "HUG",
          "itemSpacing": "breakpoints/wel/sem/spacingStatic/stack/md"
        }
      },
      "texts": {
        "parent": "textsaction",
        "children": [
          "title",
          "subtitle",
          "description"
        ],
        "styles": {
          "layoutMode": "VERTICAL",
          "layoutSizingHorizontal": "FILL",
          "layoutSizingVertical": "HUG",
          "itemSpacing": "breakpoints/wel/sem/spacingStatic/stack/xs"
        }
      },
      "title": {
        "parent": "texts",
        "styles": {
          "fills": "colorModes/wel/sem/color/on-surface-mid",
          "layoutSizingHorizontal": "HUG",
          "layoutSizingVertical": "HUG",
          "textStyleId": "title-03"
        }
      },
      "subtitle": {
        "parent": "texts",
        "styles": {
          "fills": "colorModes/wel/sem/color/on-surface-low",
          "layoutSizingHorizontal": "FILL",
          "layoutSizingVertical": "HUG",
          "textStyleId": "body-default-01"
        },
        "propReferences": {
          "visible": {
            "$ref": "#/props/subtitle"
          }
        }
      },
      "description": {
        "parent": "texts",
        "styles": {
          "fills": "colorModes/wel/sem/color/on-surface-mid",
          "layoutSizingHorizontal": "FILL",
          "layoutSizingVertical": "HUG",
          "textStyleId": "body-default-01"
        },
        "propReferences": {
          "visible": {
            "$ref": "#/props/description"
          }
        }
      },
      "action": {
        "parent": "textsaction",
        "styles": {
          "layoutSizingHorizontal": "HUG",
          "layoutSizingVertical": "HUG"
        },
        "propConfigurations": {
          "action": "link-icon"
        },
        "propReferences": {
          "visible": {
            "$ref": "#/props/action"
          }
        }
      }
    }
  },
  "variants": [
    {
      "name": "breakpoint=tablet (768-1023)",
      "configuration": {
        "breakpoint": "tablet (768-1023)"
      },
      "elements": {
        "root": {
          "styles": {
            "width": 396
          }
        }
      }
    },
    {
      "name": "breakpoint=desktop-sm (1024-1279)",
      "configuration": {
        "breakpoint": "desktop-sm (1024-1279)"
      },
      "elements": {
        "root": {
          "styles": {
            "width": 468
          }
        }
      }
    },
    {
      "name": "breakpoint=desktop-md (1280-1439)",
      "configuration": {
        "breakpoint": "desktop-md (1280-1439)"
      },
      "elements": {
        "root": {
          "styles": {
            "width": 564
          }
        }
      }
    }
  ],
  "invalidVariantCombinations": [],
  "metadata": {
    "author": "Arthur MATHON",
    "lastUpdated": "2025-12-04T16:04:31.997Z",
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
      "pageId": "6:764",
      "nodeId": "6:2270"
    }
  }
}