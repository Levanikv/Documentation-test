{
  "title": "aemcallout-marketing-container",
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
    "item-3": {
      "type": "instance",
      "instanceOf": "callout-marketing"
    },
    "item-1": {
      "type": "instance",
      "instanceOf": "callout-marketing"
    },
    "item-2": {
      "type": "instance",
      "instanceOf": "callout-marketing"
    },
    "webpagination-condensed": {
      "type": "instance",
      "instanceOf": "webpagination-condensed"
    },
    "item-4": {
      "type": "instance",
      "detectedIn": "breakpoint=tablet (768-1023), # columns=2, display=carousel",
      "instanceOf": "callout-marketing"
    },
    "callout-marketing": {
      "type": "instance",
      "detectedIn": "breakpoint=desktop-sm (1024-1279), # columns=2, display=carousel",
      "instanceOf": "callout-marketing"
    }
  },
  "props": {
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
    "": {
      "type": "string",
      "default": "2",
      "enum": [
        "2",
        "3",
        "4"
      ]
    },
    "display": {
      "type": "string",
      "default": "carousel",
      "enum": [
        "carousel",
        "grid"
      ]
    }
  },
  "default": {
    "name": "breakpoint=mobile (320-767), # columns=2, display=carousel",
    "elements": {
      "root": {
        "children": [
          "wrapper"
        ],
        "styles": {
          "width": 375,
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
          "item-3",
          "item-1",
          "item-2"
        ],
        "styles": {
          "width": 343,
          "primaryAxisAlignItems": "CENTER",
          "layoutMode": "HORIZONTAL",
          "layoutSizingVertical": "HUG",
          "itemSpacing": "breakpoints/wel/sem/spacingDynamic/inline/xl"
        }
      },
      "item-3": {
        "parent": "items",
        "styles": {
          "opacity": 0,
          "layoutSizingVertical": "HUG",
          "width": 311
        },
        "propConfigurations": {
          "kicker": "true",
          "description": "true",
          "background-enabled": "no"
        }
      },
      "item-1": {
        "parent": "items",
        "styles": {
          "layoutSizingVertical": "HUG",
          "width": 311
        },
        "propConfigurations": {
          "kicker": "true",
          "description": "true",
          "background-enabled": "no"
        }
      },
      "item-2": {
        "parent": "items",
        "styles": {
          "layoutSizingVertical": "HUG",
          "width": 311
        },
        "propConfigurations": {
          "kicker": "true",
          "description": "true",
          "background-enabled": "no"
        }
      },
      "webpagination-condensed": {
        "parent": "webcarousel",
        "styles": {
          "layoutSizingHorizontal": "FILL",
          "layoutSizingVertical": "HUG"
        },
        "propConfigurations": {
          "step": "1-3",
          "counter": "true",
          "size": "sm",
          "align": "right",
          "loop": "false"
        }
      },
      "item-4": {
        "styles": {
          "layoutSizingVertical": "HUG",
          "width": 340
        },
        "propConfigurations": {
          "kicker": "true",
          "description": "true",
          "background-enabled": "no"
        }
      },
      "callout-marketing": {
        "styles": {
          "layoutSizingVertical": "HUG",
          "width": 468
        },
        "propConfigurations": {
          "kicker": "true",
          "description": "true",
          "background-enabled": "no"
        }
      }
    }
  },
  "variants": [
    {
      "name": "breakpoint=mobile (320-767), # columns=3, display=carousel",
      "configuration": {
        "# columns": "3"
      },
      "elements": {
        "item-3": {
          "styles": {
            "opacity": 1
          }
        },
        "webpagination-condensed": {
          "propConfigurations": {
            "step": "1-4"
          }
        }
      }
    },
    {
      "name": "breakpoint=mobile (320-767), # columns=4, display=carousel",
      "configuration": {
        "# columns": "4"
      },
      "elements": {
        "item-3": {
          "styles": {
            "opacity": 1
          }
        },
        "webpagination-condensed": {
          "propConfigurations": {
            "step": "1-5"
          }
        }
      }
    },
    {
      "name": "breakpoint=tablet (768-1023), # columns=2, display=carousel",
      "configuration": {
        "breakpoint": "tablet (768-1023)"
      },
      "elements": {
        "root": {
          "styles": {
            "width": 768
          }
        },
        "webcarousel": {
          "styles": {
            "layoutSizingHorizontal": "FIXED",
            "width": "breakpoints/wel/sem/sizing/grid/fullGrid"
          }
        },
        "items": {
          "children": [
            "item-4",
            "item-1",
            "item-2",
            "item-3"
          ],
          "styles": {
            "layoutSizingHorizontal": "FILL"
          }
        },
        "item-4": {
          "parent": "items"
        },
        "item-3": {
          "styles": {
            "opacity": 1
          }
        },
        "webpagination-condensed": {
          "propConfigurations": {
            "size": "md"
          }
        }
      }
    },
    {
      "name": "breakpoint=desktop-sm (1024-1279), # columns=2, display=carousel",
      "configuration": {
        "breakpoint": "desktop-sm (1024-1279)"
      },
      "elements": {
        "root": {
          "styles": {
            "width": 1024
          }
        },
        "webcarousel": {
          "styles": {
            "layoutSizingHorizontal": "FIXED",
            "width": "breakpoints/wel/sem/sizing/grid/fullGrid"
          }
        },
        "items": {
          "children": [
            "callout-marketing",
            "callout-marketing",
            "callout-marketing",
            "callout-marketing"
          ],
          "styles": {
            "layoutSizingHorizontal": "FILL"
          }
        },
        "callout-marketing": {
          "parent": "items"
        },
        "webpagination-condensed": {
          "propConfigurations": {
            "size": "md"
          }
        }
      }
    },
    {
      "name": "breakpoint=desktop-md (1280-1439), # columns=2, display=carousel",
      "configuration": {
        "breakpoint": "desktop-md (1280-1439)"
      },
      "elements": {
        "root": {
          "styles": {
            "width": 1340
          }
        },
        "webcarousel": {
          "styles": {
            "layoutSizingHorizontal": "FIXED",
            "width": "breakpoints/wel/sem/sizing/grid/fullGrid"
          }
        },
        "items": {
          "children": [
            "callout-marketing",
            "callout-marketing",
            "callout-marketing",
            "callout-marketing"
          ],
          "styles": {
            "layoutSizingHorizontal": "FILL"
          }
        },
        "callout-marketing": {
          "parent": "items"
        },
        "webpagination-condensed": {
          "propConfigurations": {
            "size": "md"
          }
        }
      }
    }
  ],
  "invalidConfigurations": [
    {
      "display": "grid"
    }
  ]
}