# Design Export Context

- Generated at: `2026-03-15T04:21:36.747Z`
- Document ID: `89299321-273e-4740-83e4-cf454192bc91`
- Page count: 5

## Original Prompt

```text
You are a professional chef and nutrition expert.

A user will provide a list of ingredients they currently have. Your task is to generate a simple, delicious recipe using those ingredients.

Ingredients provided by the user:
{ingredients}

Instructions:
1. Suggest a recipe name.
2. Use the provided ingredients as much as possible.
3. You may add a few common pantry items if needed (salt, oil, spices).
4. Provide clear step-by-step cooking instructions.
5. Mention preparation time and cooking time.
6. Include a short description of the dish.

Output format:

Recipe Name:
Description:
Preparation Time:
Cooking Time:

Ingredients:
- item 1
- item 2

Instructions:
1.
2.
3.

Optional Tips:
```

## Theme (JSON)

```json
{
  "fonts": {
    "primary": "google:Plus Jakarta Sans",
    "secondary": "google:Nunito"
  },
  "colors": {
    "light": {
      "primary": "#E63946",
      "on_primary": "#FFFFFF",
      "secondary": "#4CC9F0",
      "on_secondary": "#000000",
      "accent": "#FFD60A",
      "background": "#F8F9FA",
      "surface": "#FFFFFF",
      "on_surface": "#1D1D1F",
      "primary_text": "#2B2D42",
      "secondary_text": "#8D99AE",
      "hint": "#CED4DA",
      "error": "#EF233C",
      "on_error": "#FFFFFF",
      "success": "#52B788",
      "divider": "#2B2D42",
      "transparent": "#00000000"
    },
    "dark": {
      "primary": "#F1515E",
      "on_primary": "#FFFFFF",
      "secondary": "#4CC9F0",
      "on_secondary": "#000000",
      "accent": "#FFD60A",
      "background": "#121212",
      "surface": "#1E1E1E",
      "on_surface": "#F8F9FA",
      "primary_text": "#F8F9FA",
      "secondary_text": "#ADB5BD",
      "hint": "#495057",
      "error": "#FF4D6D",
      "on_error": "#FFFFFF",
      "success": "#74C69D",
      "divider": "#F8F9FA",
      "transparent": "#00000000"
    }
  },
  "text_styles": {
    "headline_large": {
      "font": "primary",
      "size": 34,
      "weight": 800,
      "height": 1.1
    },
    "headline_medium": {
      "font": "primary",
      "size": 28,
      "weight": 800,
      "height": 1.2
    },
    "title_large": {
      "font": "primary",
      "size": 22,
      "weight": 700,
      "height": 1.2
    },
    "title_medium": {
      "font": "primary",
      "size": 18,
      "weight": 700,
      "height": 1.3
    },
    "body_large": {
      "font": "secondary",
      "size": 17,
      "weight": 600,
      "height": 1.5
    },
    "body_medium": {
      "font": "secondary",
      "size": 15,
      "weight": 600,
      "height": 1.5
    },
    "body_small": {
      "font": "secondary",
      "size": 13,
      "weight": 600,
      "height": 1.4
    },
    "label_large": {
      "font": "primary",
      "size": 15,
      "weight": 800,
      "height": 1.2
    },
    "label_medium": {
      "font": "primary",
      "size": 13,
      "weight": 800,
      "height": 1.2
    },
    "label_small": {
      "font": "primary",
      "size": 11,
      "weight": 800,
      "height": 1.2
    }
  },
  "spacing": {
    "xs": 4,
    "sm": 8,
    "md": 16,
    "lg": 24,
    "xl": 32
  },
  "radii": {
    "sm": 8,
    "md": 16,
    "lg": 28,
    "full": 9999
  },
  "shadows": {
    "sm": {
      "color": "#2B2D4233",
      "dx": 0,
      "dy": 3,
      "blur": 0,
      "spread": 0
    },
    "md": {
      "color": "#2B2D4244",
      "dx": 0,
      "dy": 5,
      "blur": 0,
      "spread": 0
    },
    "lg": {
      "color": "#2B2D4255",
      "dx": 0,
      "dy": 8,
      "blur": 0,
      "spread": 0
    },
    "xl": {
      "color": "#2B2D4266",
      "dx": 0,
      "dy": 12,
      "blur": 0,
      "spread": 0
    }
  }
}
```

## Pages

### 1. Ingredient Input

- Frame ID: `7d9b4a24-769a-45f9-a746-6d7d6c40485b`
- Original page prompt: "A screen to enter or scan available ingredients from your pantry"
- Follow-up prompts: _None_

#### DslDocument (JSON)

```json
{
  "root": {
    "type": "scaffold",
    "properties": {
      "bg": {
        "color": {
          "color": "background"
        }
      },
      "safe_area": {
        "boolVal": {
          "value": true
        }
      }
    },
    "children": [
      {
        "type": "column",
        "properties": {
          "scroll": {
            "boolVal": {
              "value": true
            }
          },
          "spacing": {
            "stringVal": {
              "value": "lg"
            }
          },
          "padding": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "token": "lg"
            }
          }
        },
        "children": [
          {
            "type": "row",
            "properties": {
              "align": {
                "align": {
                  "named": "space_between"
                }
              }
            },
            "children": [
              {
                "type": "column",
                "properties": {
                  "cross_align": {
                    "align": {
                      "named": "start"
                    }
                  },
                  "spacing": {
                    "stringVal": {
                      "value": "xs"
                    }
                  }
                },
                "children": [
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Pantry Chef"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "label_large"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary"
                        }
                      },
                      "font_weight": {
                        "stringVal": {
                          "value": "bold"
                        }
                      }
                    },
                    "editorId": "d6b34b58-9488-4d6c-b340-e6907fdba050"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "What's in your kitchen?"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "headline_medium"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      }
                    },
                    "editorId": "c055c887-d12e-4cd7-911a-5b4bc382be7f"
                  }
                ],
                "editorId": "7a223c31-c9db-476f-a504-c670c5a14037"
              },
              {
                "type": "container",
                "properties": {
                  "width": {
                    "px": {
                      "value": 48,
                      "isInfinity": false
                    }
                  },
                  "height": {
                    "px": {
                      "value": 48,
                      "isInfinity": false
                    }
                  },
                  "bg": {
                    "color": {
                      "color": "surface"
                    }
                  },
                  "radius": {
                    "radius": {
                      "topLeft": 0,
                      "topRight": 0,
                      "bottomLeft": 0,
                      "bottomRight": 0,
                      "token": "full"
                    }
                  },
                  "border": {
                    "border": {
                      "width": 2,
                      "color": "divider"
                    }
                  },
                  "clip": {
                    "boolVal": {
                      "value": true
                    }
                  }
                },
                "children": [
                  {
                    "type": "image",
                    "properties": {
                      "source_desc": {
                        "imageSource": {
                          "type": "IMAGE_SOURCE_TYPE_DESCRIPTION",
                          "value": "friendly chef avatar portrait"
                        }
                      },
                      "fit": {
                        "stringVal": {
                          "value": "cover"
                        }
                      }
                    },
                    "editorId": "5bc7df96-a7ae-4ae6-a6aa-6b1f536dfe9d"
                  }
                ],
                "editorId": "1f13d282-1c40-427e-a48c-6738f0e10c3b"
              }
            ],
            "editorId": "d3d36544-5618-40fc-8ac4-e0824a349ca1"
          },
          {
            "type": "container",
            "properties": {
              "bg": {
                "color": {
                  "color": "surface"
                }
              },
              "radius": {
                "radius": {
                  "topLeft": 0,
                  "topRight": 0,
                  "bottomLeft": 0,
                  "bottomRight": 0,
                  "token": "xl"
                }
              },
              "padding": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "token": "lg"
                }
              },
              "border": {
                "border": {
                  "width": 2,
                  "color": "divider"
                }
              },
              "shadow": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "column",
                "properties": {
                  "spacing": {
                    "stringVal": {
                      "value": "md"
                    }
                  }
                },
                "children": [
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Add Ingredients"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "title_medium"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      },
                      "font_weight": {
                        "stringVal": {
                          "value": "bold"
                        }
                      }
                    },
                    "editorId": "63cc01e2-9d3a-423e-81e0-01f08308e550"
                  },
                  {
                    "type": "row",
                    "properties": {
                      "spacing": {
                        "stringVal": {
                          "value": "md"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "expanded",
                        "children": [
                          {
                            "type": "textfield",
                            "properties": {
                              "hint": {
                                "stringVal": {
                                  "value": "Enter ingredient (e.g. Eggs)"
                                }
                              },
                              "radius": {
                                "radius": {
                                  "topLeft": 0,
                                  "topRight": 0,
                                  "bottomLeft": 0,
                                  "bottomRight": 0,
                                  "token": "lg"
                                }
                              },
                              "border": {
                                "border": {
                                  "width": 2,
                                  "color": "divider"
                                }
                              },
                              "filled": {
                                "boolVal": {
                                  "value": true
                                }
                              },
                              "bg": {
                                "color": {
                                  "color": "background"
                                }
                              },
                              "prefix_icon": {
                                "stringVal": {
                                  "value": "search_rounded"
                                }
                              }
                            },
                            "editorId": "665422c6-725e-4443-8f8a-622fc1fbd316"
                          }
                        ],
                        "editorId": "7a7d223a-6e5a-4be7-8b82-ae66cd211d1c"
                      },
                      {
                        "type": "container",
                        "properties": {
                          "width": {
                            "px": {
                              "value": 56,
                              "isInfinity": false
                            }
                          },
                          "height": {
                            "px": {
                              "value": 56,
                              "isInfinity": false
                            }
                          },
                          "bg": {
                            "color": {
                              "color": "primary"
                            }
                          },
                          "radius": {
                            "radius": {
                              "topLeft": 0,
                              "topRight": 0,
                              "bottomLeft": 0,
                              "bottomRight": 0,
                              "token": "lg"
                            }
                          },
                          "border": {
                            "border": {
                              "width": 2,
                              "color": "divider"
                            }
                          },
                          "shadow": {
                            "stringVal": {
                              "value": "sm"
                            }
                          },
                          "align_child": {
                            "align": {
                              "named": "center"
                            }
                          }
                        },
                        "children": [
                          {
                            "type": "icon",
                            "properties": {
                              "name": {
                                "icon": {
                                  "name": "add_rounded"
                                }
                              },
                              "color": {
                                "color": {
                                  "color": "on_primary"
                                }
                              },
                              "size": {
                                "numberVal": {
                                  "value": 32
                                }
                              }
                            },
                            "editorId": "7f3232e6-137f-493a-b205-36749a700769"
                          }
                        ],
                        "editorId": "28878bc9-03ab-443c-af04-70e7a0aaddd8"
                      }
                    ],
                    "editorId": "c894e453-959b-4a96-a1b0-657562ae23cf"
                  }
                ],
                "editorId": "fa742dfe-e1fa-4c6a-a004-d1be8e366975"
              }
            ],
            "editorId": "fa35db4f-4df1-42c7-a396-5742807e33ac"
          },
          {
            "type": "row",
            "properties": {
              "spacing": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "@quick_action",
                "properties": {
                  "bg": {
                    "stringVal": {
                      "value": "accent"
                    }
                  },
                  "icon": {
                    "stringVal": {
                      "value": "camera_alt_rounded"
                    }
                  },
                  "label": {
                    "stringVal": {
                      "value": "Scan Receipt"
                    }
                  }
                },
                "editorId": "fb3dbf64-a2e8-43e5-8335-ce31e179d807"
              },
              {
                "type": "@quick_action",
                "properties": {
                  "bg": {
                    "stringVal": {
                      "value": "secondary"
                    }
                  },
                  "icon": {
                    "stringVal": {
                      "value": "center_focus_weak_rounded"
                    }
                  },
                  "label": {
                    "stringVal": {
                      "value": "AI Vision"
                    }
                  }
                },
                "editorId": "d81bd967-ffe0-42c3-83f3-f88f00b8bef4"
              }
            ],
            "editorId": "70463030-ed24-4476-b581-e72f5717e9d5"
          },
          {
            "type": "column",
            "properties": {
              "cross_align": {
                "align": {
                  "named": "stretch"
                }
              },
              "spacing": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "row",
                "properties": {
                  "align": {
                    "align": {
                      "named": "space_between"
                    }
                  }
                },
                "children": [
                  {
                    "type": "row",
                    "properties": {
                      "spacing": {
                        "stringVal": {
                          "value": "sm"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "icon",
                        "properties": {
                          "name": {
                            "icon": {
                              "name": "restaurant_menu_rounded"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary"
                            }
                          },
                          "size": {
                            "numberVal": {
                              "value": 24
                            }
                          }
                        },
                        "editorId": "bd835023-0d4b-47b8-b35a-4f9eaca70dc7"
                      },
                      {
                        "type": "text",
                        "properties": {
                          "content": {
                            "stringVal": {
                              "value": "Your Ingredients (6)"
                            }
                          },
                          "style": {
                            "textStyle": {
                              "styleName": "title_large"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary_text"
                            }
                          }
                        },
                        "editorId": "4bfd8d76-6761-4bff-b2c4-31e0e16887f9"
                      }
                    ],
                    "editorId": "06335f15-639b-40a8-b937-1f5575f186f3"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Clear All"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "label_large"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "secondary_text"
                        }
                      }
                    },
                    "editorId": "2d21cc56-080d-4662-99b1-1bc006c24f5e"
                  }
                ],
                "editorId": "6311d2d7-4895-4c3c-9d76-5b66aa3dd939"
              },
              {
                "type": "column",
                "properties": {
                  "spacing": {
                    "numberVal": {
                      "value": 0
                    }
                  }
                },
                "children": [
                  {
                    "type": "@ingredient_pill",
                    "properties": {
                      "name": {
                        "stringVal": {
                          "value": "Farm Fresh Eggs"
                        }
                      },
                      "category": {
                        "stringVal": {
                          "value": "Protein"
                        }
                      },
                      "icon": {
                        "stringVal": {
                          "value": "egg_rounded"
                        }
                      },
                      "color": {
                        "stringVal": {
                          "value": "accent"
                        }
                      }
                    },
                    "editorId": "1978ad06-a66d-447a-baa2-45c0f1fdf032"
                  },
                  {
                    "type": "@ingredient_pill",
                    "properties": {
                      "name": {
                        "stringVal": {
                          "value": "Russet Potatoes"
                        }
                      },
                      "category": {
                        "stringVal": {
                          "value": "Vegetables"
                        }
                      },
                      "icon": {
                        "stringVal": {
                          "value": "kitchen_rounded"
                        }
                      },
                      "color": {
                        "stringVal": {
                          "value": "secondary"
                        }
                      }
                    },
                    "editorId": "16b442f3-997d-49d0-a0b2-4ed5b0c1a311"
                  },
                  {
                    "type": "@ingredient_pill",
                    "properties": {
                      "name": {
                        "stringVal": {
                          "value": "Red Onion"
                        }
                      },
                      "category": {
                        "stringVal": {
                          "value": "Vegetables"
                        }
                      },
                      "icon": {
                        "stringVal": {
                          "value": "outdoor_grill_rounded"
                        }
                      },
                      "color": {
                        "stringVal": {
                          "value": "secondary"
                        }
                      }
                    },
                    "editorId": "18e0651b-dadc-4143-8020-9d876b553335"
                  },
                  {
                    "type": "@ingredient_pill",
                    "properties": {
                      "name": {
                        "stringVal": {
                          "value": "Baby Spinach"
                        }
                      },
                      "category": {
                        "stringVal": {
                          "value": "Greens"
                        }
                      },
                      "icon": {
                        "stringVal": {
                          "value": "eco_rounded"
                        }
                      },
                      "color": {
                        "stringVal": {
                          "value": "success"
                        }
                      }
                    },
                    "editorId": "52710ba6-8681-4a8c-81e9-a7e178666a5f"
                  },
                  {
                    "type": "@ingredient_pill",
                    "properties": {
                      "name": {
                        "stringVal": {
                          "value": "Cheddar Cheese"
                        }
                      },
                      "category": {
                        "stringVal": {
                          "value": "Dairy"
                        }
                      },
                      "icon": {
                        "stringVal": {
                          "value": "breakfast_dining_rounded"
                        }
                      },
                      "color": {
                        "stringVal": {
                          "value": "accent"
                        }
                      }
                    },
                    "editorId": "e2fce721-66e5-49ff-8cae-13b60263af48"
                  },
                  {
                    "type": "@ingredient_pill",
                    "properties": {
                      "name": {
                        "stringVal": {
                          "value": "Garlic Cloves"
                        }
                      },
                      "category": {
                        "stringVal": {
                          "value": "Pantry"
                        }
                      },
                      "icon": {
                        "stringVal": {
                          "value": "grain_rounded"
                        }
                      },
                      "color": {
                        "stringVal": {
                          "value": "divider"
                        }
                      }
                    },
                    "editorId": "982f8a36-88c2-44bc-a390-f5455d0e588e"
                  }
                ],
                "editorId": "6f3a47c5-e7e8-482b-9b67-60f5707a00a9"
              }
            ],
            "editorId": "f0613bb3-5612-4d33-a0f3-9c225e37bd86"
          },
          {
            "type": "column",
            "properties": {
              "cross_align": {
                "align": {
                  "named": "start"
                }
              },
              "spacing": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "text",
                "properties": {
                  "content": {
                    "stringVal": {
                      "value": "Common Staples"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "title_medium"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  }
                },
                "editorId": "d412bcab-1eeb-4b4f-a324-e770bc1fb890"
              },
              {
                "type": "wrap",
                "properties": {
                  "spacing": {
                    "stringVal": {
                      "value": "md"
                    }
                  },
                  "run_spacing": {
                    "stringVal": {
                      "value": "md"
                    }
                  }
                },
                "children": [
                  {
                    "type": "chip",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Olive Oil"
                        }
                      },
                      "icon": {
                        "icon": {
                          "name": "check_circle_rounded"
                        }
                      },
                      "selected": {
                        "boolVal": {
                          "value": true
                        }
                      },
                      "bg": {
                        "color": {
                          "color": "surface"
                        }
                      },
                      "border": {
                        "border": {
                          "width": 2,
                          "color": "divider"
                        }
                      }
                    },
                    "editorId": "2f74dde4-0eaa-4a01-8111-286d3239c4fb"
                  },
                  {
                    "type": "chip",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Salt"
                        }
                      },
                      "icon": {
                        "icon": {
                          "name": "check_circle_rounded"
                        }
                      },
                      "selected": {
                        "boolVal": {
                          "value": true
                        }
                      },
                      "bg": {
                        "color": {
                          "color": "surface"
                        }
                      },
                      "border": {
                        "border": {
                          "width": 2,
                          "color": "divider"
                        }
                      }
                    },
                    "editorId": "50af4010-2a42-4dfb-9f25-1e42d111ef1d"
                  },
                  {
                    "type": "chip",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Pepper"
                        }
                      },
                      "icon": {
                        "icon": {
                          "name": "check_circle_rounded"
                        }
                      },
                      "selected": {
                        "boolVal": {
                          "value": true
                        }
                      },
                      "bg": {
                        "color": {
                          "color": "surface"
                        }
                      },
                      "border": {
                        "border": {
                          "width": 2,
                          "color": "divider"
                        }
                      }
                    },
                    "editorId": "9176b2b3-4166-4691-840d-1336fda022d1"
                  },
                  {
                    "type": "chip",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Butter"
                        }
                      },
                      "variant": {
                        "stringVal": {
                          "value": "filter"
                        }
                      },
                      "bg": {
                        "color": {
                          "color": "surface"
                        }
                      },
                      "border": {
                        "border": {
                          "width": 2,
                          "color": "divider"
                        }
                      }
                    },
                    "editorId": "f43788a7-0a41-48df-9e4a-efcf26a3894e"
                  },
                  {
                    "type": "chip",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Milk"
                        }
                      },
                      "variant": {
                        "stringVal": {
                          "value": "filter"
                        }
                      },
                      "bg": {
                        "color": {
                          "color": "surface"
                        }
                      },
                      "border": {
                        "border": {
                          "width": 2,
                          "color": "divider"
                        }
                      }
                    },
                    "editorId": "3c46807a-a3a3-4340-a469-5517fa0e55d4"
                  }
                ],
                "editorId": "2df2e615-b0f4-4789-9d82-e6dac4c6926c"
              }
            ],
            "editorId": "1e4b8a98-445d-4390-b12a-413273aad2b1"
          },
          {
            "type": "sizedbox",
            "properties": {
              "height": {
                "stringVal": {
                  "value": "lg"
                }
              }
            },
            "editorId": "b00ce73b-631b-4e7a-8279-8bb805538238"
          },
          {
            "type": "container",
            "properties": {
              "bg": {
                "color": {
                  "color": "primary"
                }
              },
              "radius": {
                "radius": {
                  "topLeft": 0,
                  "topRight": 0,
                  "bottomLeft": 0,
                  "bottomRight": 0,
                  "token": "xl"
                }
              },
              "padding": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "topToken": "xl",
                  "rightToken": "lg",
                  "bottomToken": "xl",
                  "leftToken": "lg"
                }
              },
              "border": {
                "border": {
                  "width": 2,
                  "color": "divider"
                }
              },
              "shadow": {
                "stringVal": {
                  "value": "lg"
                }
              },
              "align_child": {
                "align": {
                  "named": "center"
                }
              }
            },
            "children": [
              {
                "type": "row",
                "properties": {
                  "main_size": {
                    "stringVal": {
                      "value": "min"
                    }
                  },
                  "spacing": {
                    "stringVal": {
                      "value": "md"
                    }
                  }
                },
                "children": [
                  {
                    "type": "icon",
                    "properties": {
                      "name": {
                        "icon": {
                          "name": "auto_awesome_rounded"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "on_primary"
                        }
                      },
                      "size": {
                        "numberVal": {
                          "value": 28
                        }
                      }
                    },
                    "editorId": "c6bad49e-fc4b-46d4-b0a6-3ef4a6d6a3e1"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Generate Magic Recipe"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "title_large"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "on_primary"
                        }
                      },
                      "font_weight": {
                        "numberVal": {
                          "value": 800
                        }
                      }
                    },
                    "editorId": "3e6aa94c-433d-4605-ba78-1fa9b905dd33"
                  }
                ],
                "editorId": "384c34e4-41fc-4836-b73d-1b5f22b81546"
              }
            ],
            "editorId": "93f172dc-c213-4396-ab26-f9f4d1e8cdc6"
          },
          {
            "type": "center",
            "children": [
              {
                "type": "text",
                "properties": {
                  "content": {
                    "stringVal": {
                      "value": "Chef will use your ingredients + basic staples"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "body_small"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "secondary_text"
                    }
                  }
                },
                "editorId": "48bf2aa5-4772-48cd-8f9a-ec5d70bfe77a"
              }
            ],
            "editorId": "fd33de13-373c-4c91-9092-e593788a1a67"
          },
          {
            "type": "sizedbox",
            "properties": {
              "height": {
                "stringVal": {
                  "value": "xl"
                }
              }
            },
            "editorId": "f5a7aa2b-11ec-4ebd-9e33-fe7cb6448878"
          }
        ],
        "editorId": "c0eb3918-1af2-4a42-9793-8e5002db5228"
      }
    ],
    "editorId": "47824d33-f187-42e4-bd91-1e426ca3a680"
  },
  "components": [
    {
      "name": "ingredient_pill",
      "root": {
        "type": "container",
        "properties": {
          "bg": {
            "color": {
              "color": "surface"
            }
          },
          "radius": {
            "radius": {
              "topLeft": 0,
              "topRight": 0,
              "bottomLeft": 0,
              "bottomRight": 0,
              "token": "lg"
            }
          },
          "padding": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "token": "md"
            }
          },
          "border": {
            "border": {
              "width": 2,
              "color": "divider"
            }
          },
          "margin": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "bottomToken": "md"
            }
          },
          "shadow": {
            "stringVal": {
              "value": "sm"
            }
          }
        },
        "children": [
          {
            "type": "row",
            "properties": {
              "spacing": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "container",
                "properties": {
                  "width": {
                    "px": {
                      "value": 40,
                      "isInfinity": false
                    }
                  },
                  "height": {
                    "px": {
                      "value": 40,
                      "isInfinity": false
                    }
                  },
                  "bg": {
                    "slot": {
                      "name": "color"
                    }
                  },
                  "radius": {
                    "radius": {
                      "topLeft": 0,
                      "topRight": 0,
                      "bottomLeft": 0,
                      "bottomRight": 0,
                      "token": "md"
                    }
                  },
                  "border": {
                    "border": {
                      "width": 2,
                      "color": "divider"
                    }
                  },
                  "align_child": {
                    "align": {
                      "named": "center"
                    }
                  }
                },
                "children": [
                  {
                    "type": "icon",
                    "properties": {
                      "name": {
                        "slot": {
                          "name": "icon"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      },
                      "size": {
                        "numberVal": {
                          "value": 20
                        }
                      }
                    },
                    "editorId": "3147404a-7572-48e2-8622-cfa39e15d871"
                  }
                ],
                "editorId": "4a3a0864-a9c5-43c6-a1c4-36b33f3d9fb9"
              },
              {
                "type": "expanded",
                "children": [
                  {
                    "type": "column",
                    "properties": {
                      "cross_align": {
                        "align": {
                          "named": "start"
                        }
                      },
                      "spacing": {
                        "numberVal": {
                          "value": 2
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "text",
                        "properties": {
                          "content": {
                            "slot": {
                              "name": "name"
                            }
                          },
                          "style": {
                            "textStyle": {
                              "styleName": "title_medium"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary_text"
                            }
                          },
                          "max_lines": {
                            "numberVal": {
                              "value": 1
                            }
                          },
                          "overflow": {
                            "stringVal": {
                              "value": "ellipsis"
                            }
                          }
                        },
                        "editorId": "b6877010-b234-4b19-848a-c495a5c9f521"
                      },
                      {
                        "type": "text",
                        "properties": {
                          "content": {
                            "slot": {
                              "name": "category"
                            }
                          },
                          "style": {
                            "textStyle": {
                              "styleName": "label_small"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "secondary_text"
                            }
                          }
                        },
                        "editorId": "2cda8e20-520c-4632-adc6-6c6597262504"
                      }
                    ],
                    "editorId": "1b4d88cd-d628-4288-9aa1-93300de1d9ab"
                  }
                ],
                "editorId": "9939ac6f-64c9-4e01-aa54-0366e292480f"
              },
              {
                "type": "iconbutton",
                "properties": {
                  "name": {
                    "icon": {
                      "name": "remove_circle_outline_rounded"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "error"
                    }
                  },
                  "size": {
                    "numberVal": {
                      "value": 24
                    }
                  }
                },
                "editorId": "cf68d51e-14fe-438b-84cb-3e0c95a62ff5"
              }
            ],
            "editorId": "6b088c6b-cb27-4990-b1c4-0bde6133f1b0"
          }
        ],
        "editorId": "3d1ab38d-a7f8-414a-ba68-42ae7fc48144"
      }
    },
    {
      "name": "quick_action",
      "root": {
        "type": "expanded",
        "children": [
          {
            "type": "container",
            "properties": {
              "bg": {
                "slot": {
                  "name": "bg"
                }
              },
              "radius": {
                "radius": {
                  "topLeft": 0,
                  "topRight": 0,
                  "bottomLeft": 0,
                  "bottomRight": 0,
                  "token": "xl"
                }
              },
              "padding": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "token": "lg"
                }
              },
              "border": {
                "border": {
                  "width": 2,
                  "color": "divider"
                }
              },
              "shadow": {
                "stringVal": {
                  "value": "md"
                }
              },
              "height": {
                "px": {
                  "value": 120,
                  "isInfinity": false
                }
              }
            },
            "children": [
              {
                "type": "column",
                "properties": {
                  "align": {
                    "align": {
                      "named": "center"
                    }
                  },
                  "spacing": {
                    "stringVal": {
                      "value": "sm"
                    }
                  }
                },
                "children": [
                  {
                    "type": "icon",
                    "properties": {
                      "name": {
                        "slot": {
                          "name": "icon"
                        }
                      },
                      "size": {
                        "numberVal": {
                          "value": 32
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      }
                    },
                    "editorId": "3d4b16b0-63e4-4737-9b39-6556134d2cad"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "slot": {
                          "name": "label"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "label_large"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      },
                      "font_weight": {
                        "stringVal": {
                          "value": "bold"
                        }
                      }
                    },
                    "editorId": "52806cd1-a0d4-4e29-a19e-34392407af44"
                  }
                ],
                "editorId": "0bee1175-51a3-478d-9c8c-4dc1dacdfd70"
              }
            ],
            "editorId": "5d7cd5d9-40b7-4b4c-b05c-4f44bd26b257"
          }
        ],
        "editorId": "65333c40-e422-42c8-b6cd-74082674753f"
      }
    }
  ]
}
```

### 2. Recipe Discovery

- Frame ID: `f1fd6b80-6861-4e6c-b1d8-9ed855c118e1`
- Original page prompt: "A feed of suggested recipes based on the ingredients provided"
- Follow-up prompts: _None_

#### DslDocument (JSON)

```json
{
  "root": {
    "type": "scaffold",
    "properties": {
      "bg": {
        "color": {
          "color": "background"
        }
      },
      "safe_area": {
        "boolVal": {
          "value": true
        }
      }
    },
    "children": [
      {
        "type": "column",
        "properties": {
          "scroll": {
            "boolVal": {
              "value": true
            }
          },
          "spacing": {
            "stringVal": {
              "value": "lg"
            }
          },
          "padding": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "token": "lg"
            }
          }
        },
        "children": [
          {
            "type": "row",
            "properties": {
              "align": {
                "align": {
                  "named": "space_between"
                }
              }
            },
            "children": [
              {
                "type": "column",
                "properties": {
                  "cross_align": {
                    "align": {
                      "named": "start"
                    }
                  },
                  "spacing": {
                    "stringVal": {
                      "value": "xs"
                    }
                  }
                },
                "children": [
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Pantry Chef"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "label_large"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary"
                        }
                      }
                    },
                    "editorId": "d5f3a475-d873-43e3-8dd0-7ae6e9040629"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Recipe Discovery"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "headline_medium"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      }
                    },
                    "editorId": "22b0433d-6dfa-40ad-a477-e85f036dd3df"
                  }
                ],
                "editorId": "39502c72-5596-436e-bd96-3504ff9c84ce"
              },
              {
                "type": "container",
                "properties": {
                  "width": {
                    "px": {
                      "value": 48,
                      "isInfinity": false
                    }
                  },
                  "height": {
                    "px": {
                      "value": 48,
                      "isInfinity": false
                    }
                  },
                  "bg": {
                    "color": {
                      "color": "surface"
                    }
                  },
                  "radius": {
                    "radius": {
                      "topLeft": 0,
                      "topRight": 0,
                      "bottomLeft": 0,
                      "bottomRight": 0,
                      "token": "lg"
                    }
                  },
                  "border": {
                    "border": {
                      "width": 2,
                      "color": "divider"
                    }
                  },
                  "align_child": {
                    "align": {
                      "named": "center"
                    }
                  }
                },
                "children": [
                  {
                    "type": "icon",
                    "properties": {
                      "name": {
                        "icon": {
                          "name": "tune_rounded"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      }
                    },
                    "editorId": "8c349354-7047-4b54-a476-c6e428166845"
                  }
                ],
                "editorId": "8c3afb2a-d8c4-4bc5-a410-8190eac01e77"
              }
            ],
            "editorId": "522d7f14-180b-4d50-9560-3a4182020965"
          },
          {
            "type": "container",
            "properties": {
              "bg": {
                "color": {
                  "color": "accent"
                }
              },
              "radius": {
                "radius": {
                  "topLeft": 0,
                  "topRight": 0,
                  "bottomLeft": 0,
                  "bottomRight": 0,
                  "token": "xl"
                }
              },
              "padding": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "token": "lg"
                }
              },
              "border": {
                "border": {
                  "width": 3,
                  "color": "divider"
                }
              },
              "shadow": {
                "stringVal": {
                  "value": "sm"
                }
              }
            },
            "children": [
              {
                "type": "column",
                "properties": {
                  "cross_align": {
                    "align": {
                      "named": "start"
                    }
                  },
                  "spacing": {
                    "stringVal": {
                      "value": "md"
                    }
                  }
                },
                "children": [
                  {
                    "type": "row",
                    "properties": {
                      "spacing": {
                        "stringVal": {
                          "value": "sm"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "icon",
                        "properties": {
                          "name": {
                            "icon": {
                              "name": "inventory_2_rounded"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary_text"
                            }
                          }
                        },
                        "editorId": "0cddf56c-a015-43ac-838f-9dba756bf79a"
                      },
                      {
                        "type": "text",
                        "properties": {
                          "content": {
                            "stringVal": {
                              "value": "Using your ingredients:"
                            }
                          },
                          "style": {
                            "textStyle": {
                              "styleName": "title_medium"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary_text"
                            }
                          }
                        },
                        "editorId": "a35dcc46-1942-4b72-9d04-d3d6e8047f97"
                      }
                    ],
                    "editorId": "b83ad5d3-7c77-4f20-aa93-60a925a2e941"
                  },
                  {
                    "type": "wrap",
                    "properties": {
                      "spacing": {
                        "stringVal": {
                          "value": "sm"
                        }
                      },
                      "run_spacing": {
                        "stringVal": {
                          "value": "sm"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "@filter_chip",
                        "properties": {
                          "label": {
                            "stringVal": {
                              "value": "Potatoes"
                            }
                          },
                          "icon": {
                            "stringVal": {
                              "value": "check_circle_rounded"
                            }
                          },
                          "selected": {
                            "boolVal": {
                              "value": true
                            }
                          }
                        },
                        "editorId": "3a2a4b4e-7e06-489d-a862-7066544e7e18"
                      },
                      {
                        "type": "@filter_chip",
                        "properties": {
                          "label": {
                            "stringVal": {
                              "value": "Eggs"
                            }
                          },
                          "icon": {
                            "stringVal": {
                              "value": "check_circle_rounded"
                            }
                          },
                          "selected": {
                            "boolVal": {
                              "value": true
                            }
                          }
                        },
                        "editorId": "af75597d-752f-4e0e-8a11-65bd304a2f65"
                      },
                      {
                        "type": "@filter_chip",
                        "properties": {
                          "label": {
                            "stringVal": {
                              "value": "Onion"
                            }
                          },
                          "icon": {
                            "stringVal": {
                              "value": "check_circle_rounded"
                            }
                          },
                          "selected": {
                            "boolVal": {
                              "value": true
                            }
                          }
                        },
                        "editorId": "16d39dc5-0a78-44d2-9cf8-47a74860d3e5"
                      },
                      {
                        "type": "@filter_chip",
                        "properties": {
                          "label": {
                            "stringVal": {
                              "value": "+ 2 more"
                            }
                          },
                          "icon": {
                            "stringVal": {
                              "value": "add_circle_rounded"
                            }
                          },
                          "selected": {
                            "boolVal": {
                              "value": false
                            }
                          }
                        },
                        "editorId": "f12b8460-7c01-478a-ac0d-54cf2c692296"
                      }
                    ],
                    "editorId": "94d4c462-04d6-48d9-a606-8d8318f11a63"
                  }
                ],
                "editorId": "cb13010f-19a1-41b0-92a9-f0d7cc82c16e"
              }
            ],
            "editorId": "719a02c6-4887-462e-8c98-ae3ad9614181"
          },
          {
            "type": "container",
            "properties": {
              "bg": {
                "color": {
                  "color": "surface"
                }
              },
              "radius": {
                "radius": {
                  "topLeft": 0,
                  "topRight": 0,
                  "bottomLeft": 0,
                  "bottomRight": 0,
                  "token": "xl"
                }
              },
              "padding": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "token": "lg"
                }
              },
              "border": {
                "border": {
                  "width": 3,
                  "color": "divider"
                }
              }
            },
            "children": [
              {
                "type": "column",
                "properties": {
                  "cross_align": {
                    "align": {
                      "named": "start"
                    }
                  },
                  "spacing": {
                    "stringVal": {
                      "value": "md"
                    }
                  }
                },
                "children": [
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Pantry Match Score"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "title_medium"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      }
                    },
                    "editorId": "295bf3ca-884c-465a-8645-a2cfbd7d3de2"
                  },
                  {
                    "type": "container",
                    "properties": {
                      "height": {
                        "px": {
                          "value": 120,
                          "isInfinity": false
                        }
                      },
                      "width": {
                        "px": {
                          "value": "Infinity",
                          "isInfinity": true
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "bar_chart",
                        "properties": {
                          "data": {
                            "stringVal": {
                              "value": "90,75,40"
                            }
                          },
                          "labels": {
                            "stringVal": {
                              "value": "Skillet,Omelet,Stew"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary"
                            }
                          },
                          "bar_width": {
                            "numberVal": {
                              "value": 40
                            }
                          },
                          "bar_radius": {
                            "numberVal": {
                              "value": 8
                            }
                          },
                          "show_labels": {
                            "boolVal": {
                              "value": true
                            }
                          }
                        },
                        "editorId": "d31786ea-3436-4194-9c80-7071ae74a226"
                      }
                    ],
                    "editorId": "2c822896-f52b-499a-bf2b-ea6d2cbe0a35"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "We found 3 recipes that use over 80% of your items!"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "body_small"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "secondary_text"
                        }
                      }
                    },
                    "editorId": "7b989747-578a-418b-b375-16a535830edd"
                  }
                ],
                "editorId": "d1e0356d-c321-40c5-a421-4fad522f6dc0"
              }
            ],
            "editorId": "05c548ea-f1c1-45f2-b522-72ddca0f5ca2"
          },
          {
            "type": "row",
            "properties": {
              "align": {
                "align": {
                  "named": "space_between"
                }
              }
            },
            "children": [
              {
                "type": "text",
                "properties": {
                  "content": {
                    "stringVal": {
                      "value": "Suggested for You"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "title_large"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  }
                },
                "editorId": "803dafec-ca12-49d1-be57-5d643e4495ad"
              },
              {
                "type": "text",
                "properties": {
                  "content": {
                    "stringVal": {
                      "value": "See All"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "label_large"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary"
                    }
                  }
                },
                "editorId": "b16d7d48-0a11-43a8-9407-8db5144d274e"
              }
            ],
            "editorId": "55787cde-7677-44a9-9b29-1987cdf6c230"
          },
          {
            "type": "column",
            "properties": {
              "cross_align": {
                "align": {
                  "named": "stretch"
                }
              }
            },
            "children": [
              {
                "type": "@recipe_card",
                "properties": {
                  "title": {
                    "stringVal": {
                      "value": "Golden Potato Hash"
                    }
                  },
                  "img_desc": {
                    "stringVal": {
                      "value": "crispy diced potatoes with herbs in a cast iron skillet"
                    }
                  },
                  "rating": {
                    "stringVal": {
                      "value": "4.8"
                    }
                  },
                  "match_label": {
                    "stringVal": {
                      "value": "95% Match"
                    }
                  },
                  "match_color": {
                    "stringVal": {
                      "value": "success"
                    }
                  },
                  "description": {
                    "stringVal": {
                      "value": "The ultimate comfort food. Crispy potatoes sautéed with caramelized onions and topped with perfectly set eggs."
                    }
                  },
                  "time": {
                    "stringVal": {
                      "value": "25 min"
                    }
                  },
                  "difficulty": {
                    "stringVal": {
                      "value": "Easy"
                    }
                  }
                },
                "editorId": "669a2dde-9951-4b18-86ba-43c1c0a0de9f"
              },
              {
                "type": "@recipe_card",
                "properties": {
                  "title": {
                    "stringVal": {
                      "value": "Rustic Spanish Tortilla"
                    }
                  },
                  "img_desc": {
                    "stringVal": {
                      "value": "thick spanish omelet with sliced potatoes and onions"
                    }
                  },
                  "rating": {
                    "stringVal": {
                      "value": "4.6"
                    }
                  },
                  "match_label": {
                    "stringVal": {
                      "value": "80% Match"
                    }
                  },
                  "match_color": {
                    "stringVal": {
                      "value": "secondary"
                    }
                  },
                  "description": {
                    "stringVal": {
                      "value": "A classic thick omelet made with thinly sliced potatoes and onions. Great hot or cold for any meal."
                    }
                  },
                  "time": {
                    "stringVal": {
                      "value": "35 min"
                    }
                  },
                  "difficulty": {
                    "stringVal": {
                      "value": "Medium"
                    }
                  }
                },
                "editorId": "593f9a4f-6604-4359-a871-03099678d967"
              },
              {
                "type": "@recipe_card",
                "properties": {
                  "title": {
                    "stringVal": {
                      "value": "Pantry Root Stew"
                    }
                  },
                  "img_desc": {
                    "stringVal": {
                      "value": "steaming bowl of vegetable stew with large potato chunks"
                    }
                  },
                  "rating": {
                    "stringVal": {
                      "value": "4.3"
                    }
                  },
                  "match_label": {
                    "stringVal": {
                      "value": "60% Match"
                    }
                  },
                  "match_color": {
                    "stringVal": {
                      "value": "accent"
                    }
                  },
                  "description": {
                    "stringVal": {
                      "value": "A warming, hearty stew that makes the most of your root vegetables. Simple, filling, and nutritious."
                    }
                  },
                  "time": {
                    "stringVal": {
                      "value": "45 min"
                    }
                  },
                  "difficulty": {
                    "stringVal": {
                      "value": "Easy"
                    }
                  }
                },
                "editorId": "9fc69b5a-adc2-4ebc-9e1f-2a2ac7993551"
              }
            ],
            "editorId": "41acf3aa-9c37-4b68-91f7-8e8a2432b782"
          },
          {
            "type": "container",
            "properties": {
              "bg": {
                "color": {
                  "color": "secondary"
                }
              },
              "radius": {
                "radius": {
                  "topLeft": 0,
                  "topRight": 0,
                  "bottomLeft": 0,
                  "bottomRight": 0,
                  "token": "xl"
                }
              },
              "padding": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "token": "lg"
                }
              },
              "border": {
                "border": {
                  "width": 3,
                  "color": "divider"
                }
              },
              "shadow": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "row",
                "properties": {
                  "spacing": {
                    "stringVal": {
                      "value": "md"
                    }
                  }
                },
                "children": [
                  {
                    "type": "container",
                    "properties": {
                      "width": {
                        "px": {
                          "value": 50,
                          "isInfinity": false
                        }
                      },
                      "height": {
                        "px": {
                          "value": 50,
                          "isInfinity": false
                        }
                      },
                      "bg": {
                        "color": {
                          "color": "surface"
                        }
                      },
                      "radius": {
                        "radius": {
                          "topLeft": 0,
                          "topRight": 0,
                          "bottomLeft": 0,
                          "bottomRight": 0,
                          "token": "full"
                        }
                      },
                      "border": {
                        "border": {
                          "width": 2,
                          "color": "divider"
                        }
                      },
                      "align_child": {
                        "align": {
                          "named": "center"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "icon",
                        "properties": {
                          "name": {
                            "icon": {
                              "name": "auto_awesome_rounded"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary"
                            }
                          },
                          "size": {
                            "numberVal": {
                              "value": 24
                            }
                          }
                        },
                        "editorId": "18742652-f447-4231-a2f6-70980cc1170b"
                      }
                    ],
                    "editorId": "47e544ce-21d0-4014-9f52-fff57048bad7"
                  },
                  {
                    "type": "expanded",
                    "children": [
                      {
                        "type": "column",
                        "properties": {
                          "cross_align": {
                            "align": {
                              "named": "start"
                            }
                          }
                        },
                        "children": [
                          {
                            "type": "text",
                            "properties": {
                              "content": {
                                "stringVal": {
                                  "value": "Missing something?"
                                }
                              },
                              "style": {
                                "textStyle": {
                                  "styleName": "title_medium"
                                }
                              },
                              "color": {
                                "color": {
                                  "color": "primary_text"
                                }
                              }
                            },
                            "editorId": "05981ca5-0bd0-4f1d-b25f-df4b91ce7bfd"
                          },
                          {
                            "type": "text",
                            "properties": {
                              "content": {
                                "stringVal": {
                                  "value": "We can suggest 12 more recipes if you add 'Milk' to your pantry."
                                }
                              },
                              "style": {
                                "textStyle": {
                                  "styleName": "body_small"
                                }
                              },
                              "color": {
                                "color": {
                                  "color": "primary_text"
                                }
                              }
                            },
                            "editorId": "db8b880c-ba78-45ef-bf8b-393d5003d78f"
                          }
                        ],
                        "editorId": "ca5ad761-18cc-4b90-83d5-f13fcbf4d6da"
                      }
                    ],
                    "editorId": "eb4fda3e-005b-43e9-af4e-a71a63d3d6d0"
                  },
                  {
                    "type": "icon",
                    "properties": {
                      "name": {
                        "icon": {
                          "name": "arrow_forward_rounded"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      }
                    },
                    "editorId": "22eb5259-fe97-4efe-a2b3-cc33a94f1f5c"
                  }
                ],
                "editorId": "2b5ed1ac-fb8b-4821-9ed5-f9ba106806cf"
              }
            ],
            "editorId": "acd5dd8b-c246-4ab7-a87e-2b6cc2a8291c"
          },
          {
            "type": "sizedbox",
            "properties": {
              "height": {
                "stringVal": {
                  "value": "xl"
                }
              }
            },
            "editorId": "a990a6c1-36bc-498f-a89e-f001abbbe74b"
          }
        ],
        "editorId": "6b19eff0-03ac-4ecb-948f-4c5108317ad3"
      }
    ],
    "editorId": "cdac210b-f322-40e9-b4d2-9764a27c61ee"
  },
  "components": [
    {
      "name": "recipe_card",
      "root": {
        "type": "container",
        "properties": {
          "bg": {
            "color": {
              "color": "surface"
            }
          },
          "radius": {
            "radius": {
              "topLeft": 0,
              "topRight": 0,
              "bottomLeft": 0,
              "bottomRight": 0,
              "token": "xl"
            }
          },
          "border": {
            "border": {
              "width": 3,
              "color": "divider"
            }
          },
          "shadow": {
            "stringVal": {
              "value": "md"
            }
          },
          "margin": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "bottomToken": "lg"
            }
          },
          "clip": {
            "boolVal": {
              "value": true
            }
          }
        },
        "children": [
          {
            "type": "column",
            "properties": {
              "cross_align": {
                "align": {
                  "named": "stretch"
                }
              }
            },
            "children": [
              {
                "type": "stack",
                "children": [
                  {
                    "type": "image",
                    "properties": {
                      "source_desc": {
                        "slot": {
                          "name": "img_desc"
                        }
                      },
                      "height": {
                        "px": {
                          "value": 180,
                          "isInfinity": false
                        }
                      },
                      "width": {
                        "px": {
                          "value": "Infinity",
                          "isInfinity": true
                        }
                      },
                      "fit": {
                        "stringVal": {
                          "value": "cover"
                        }
                      }
                    },
                    "editorId": "5a06ad36-4de0-4048-a135-f7db22485daf"
                  },
                  {
                    "type": "container",
                    "properties": {
                      "align": {
                        "align": {
                          "named": "top_right"
                        }
                      },
                      "padding": {
                        "edgeInsets": {
                          "top": 0,
                          "right": 0,
                          "bottom": 0,
                          "left": 0,
                          "token": "md"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "container",
                        "properties": {
                          "bg": {
                            "color": {
                              "color": "surface"
                            }
                          },
                          "radius": {
                            "radius": {
                              "topLeft": 0,
                              "topRight": 0,
                              "bottomLeft": 0,
                              "bottomRight": 0,
                              "token": "lg"
                            }
                          },
                          "padding": {
                            "edgeInsets": {
                              "top": 0,
                              "right": 0,
                              "bottom": 0,
                              "left": 0,
                              "topToken": "sm",
                              "rightToken": "md",
                              "bottomToken": "sm",
                              "leftToken": "md"
                            }
                          },
                          "border": {
                            "border": {
                              "width": 2,
                              "color": "divider"
                            }
                          }
                        },
                        "children": [
                          {
                            "type": "row",
                            "properties": {
                              "spacing": {
                                "stringVal": {
                                  "value": "xs"
                                }
                              },
                              "main_size": {
                                "stringVal": {
                                  "value": "min"
                                }
                              }
                            },
                            "children": [
                              {
                                "type": "icon",
                                "properties": {
                                  "name": {
                                    "icon": {
                                      "name": "star_rounded"
                                    }
                                  },
                                  "color": {
                                    "color": {
                                      "color": "accent"
                                    }
                                  },
                                  "size": {
                                    "numberVal": {
                                      "value": 18
                                    }
                                  }
                                },
                                "editorId": "fbfa97cc-d148-400e-a7ea-5d919e8cc58c"
                              },
                              {
                                "type": "text",
                                "properties": {
                                  "content": {
                                    "slot": {
                                      "name": "rating"
                                    }
                                  },
                                  "style": {
                                    "textStyle": {
                                      "styleName": "label_large"
                                    }
                                  },
                                  "color": {
                                    "color": {
                                      "color": "primary_text"
                                    }
                                  }
                                },
                                "editorId": "5dfa2c28-0fcf-4895-90d0-0133bb19cb19"
                              }
                            ],
                            "editorId": "87afb5fa-6f4e-486f-a190-16b88fff5e01"
                          }
                        ],
                        "editorId": "b40bb2d7-277c-46f6-8385-8f174061c061"
                      }
                    ],
                    "editorId": "0503cb32-2b41-46f1-a513-bf1c39d64646"
                  }
                ],
                "editorId": "13d420db-e7f7-4fc2-8afb-bbe42aa06be0"
              },
              {
                "type": "container",
                "properties": {
                  "padding": {
                    "edgeInsets": {
                      "top": 0,
                      "right": 0,
                      "bottom": 0,
                      "left": 0,
                      "token": "lg"
                    }
                  }
                },
                "children": [
                  {
                    "type": "column",
                    "properties": {
                      "cross_align": {
                        "align": {
                          "named": "start"
                        }
                      },
                      "spacing": {
                        "stringVal": {
                          "value": "sm"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "row",
                        "properties": {
                          "align": {
                            "align": {
                              "named": "space_between"
                            }
                          }
                        },
                        "children": [
                          {
                            "type": "expanded",
                            "children": [
                              {
                                "type": "text",
                                "properties": {
                                  "content": {
                                    "slot": {
                                      "name": "title"
                                    }
                                  },
                                  "style": {
                                    "textStyle": {
                                      "styleName": "title_large"
                                    }
                                  },
                                  "color": {
                                    "color": {
                                      "color": "primary_text"
                                    }
                                  },
                                  "max_lines": {
                                    "numberVal": {
                                      "value": 1
                                    }
                                  },
                                  "overflow": {
                                    "stringVal": {
                                      "value": "ellipsis"
                                    }
                                  }
                                },
                                "editorId": "de904e70-d912-4d59-b924-494b4c0ef843"
                              }
                            ],
                            "editorId": "beb112e8-550f-47ff-87e1-66be61d9a23c"
                          },
                          {
                            "type": "container",
                            "properties": {
                              "bg": {
                                "slot": {
                                  "name": "match_color"
                                }
                              },
                              "radius": {
                                "radius": {
                                  "topLeft": 0,
                                  "topRight": 0,
                                  "bottomLeft": 0,
                                  "bottomRight": 0,
                                  "token": "md"
                                }
                              },
                              "padding": {
                                "edgeInsets": {
                                  "top": 0,
                                  "right": 0,
                                  "bottom": 0,
                                  "left": 0,
                                  "topToken": "xs",
                                  "rightToken": "sm",
                                  "bottomToken": "xs",
                                  "leftToken": "sm"
                                }
                              },
                              "border": {
                                "border": {
                                  "width": 2,
                                  "color": "divider"
                                }
                              }
                            },
                            "children": [
                              {
                                "type": "text",
                                "properties": {
                                  "content": {
                                    "slot": {
                                      "name": "match_label"
                                    }
                                  },
                                  "style": {
                                    "textStyle": {
                                      "styleName": "label_small"
                                    }
                                  },
                                  "color": {
                                    "color": {
                                      "color": "primary_text"
                                    }
                                  }
                                },
                                "editorId": "42a3183b-4bb3-4db8-baac-a5e704877b6c"
                              }
                            ],
                            "editorId": "947d7c35-46b4-4d73-997d-7848840937d3"
                          }
                        ],
                        "editorId": "58272bb5-2517-4442-a52a-ff0329e02f34"
                      },
                      {
                        "type": "text",
                        "properties": {
                          "content": {
                            "slot": {
                              "name": "description"
                            }
                          },
                          "style": {
                            "textStyle": {
                              "styleName": "body_medium"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "secondary_text"
                            }
                          },
                          "max_lines": {
                            "numberVal": {
                              "value": 2
                            }
                          },
                          "overflow": {
                            "stringVal": {
                              "value": "ellipsis"
                            }
                          }
                        },
                        "editorId": "ef0debe7-6d2a-4c0f-ae34-1a0ac6992308"
                      },
                      {
                        "type": "row",
                        "properties": {
                          "spacing": {
                            "stringVal": {
                              "value": "md"
                            }
                          },
                          "padding": {
                            "edgeInsets": {
                              "top": 0,
                              "right": 0,
                              "bottom": 0,
                              "left": 0,
                              "topToken": "top",
                              "rightToken": "sm",
                              "bottomToken": "top",
                              "leftToken": "sm"
                            }
                          }
                        },
                        "children": [
                          {
                            "type": "row",
                            "properties": {
                              "spacing": {
                                "stringVal": {
                                  "value": "xs"
                                }
                              }
                            },
                            "children": [
                              {
                                "type": "icon",
                                "properties": {
                                  "name": {
                                    "icon": {
                                      "name": "schedule_rounded"
                                    }
                                  },
                                  "color": {
                                    "color": {
                                      "color": "primary"
                                    }
                                  },
                                  "size": {
                                    "numberVal": {
                                      "value": 18
                                    }
                                  }
                                },
                                "editorId": "8566aa6d-56b5-42d2-a3cc-1223baf2f615"
                              },
                              {
                                "type": "text",
                                "properties": {
                                  "content": {
                                    "slot": {
                                      "name": "time"
                                    }
                                  },
                                  "style": {
                                    "textStyle": {
                                      "styleName": "label_medium"
                                    }
                                  },
                                  "color": {
                                    "color": {
                                      "color": "secondary_text"
                                    }
                                  }
                                },
                                "editorId": "45c71c44-3b33-40d8-b4f8-7cd39076901e"
                              }
                            ],
                            "editorId": "f0d8d9a0-9745-4c54-a38c-d11871a6e546"
                          },
                          {
                            "type": "row",
                            "properties": {
                              "spacing": {
                                "stringVal": {
                                  "value": "xs"
                                }
                              }
                            },
                            "children": [
                              {
                                "type": "icon",
                                "properties": {
                                  "name": {
                                    "icon": {
                                      "name": "local_fire_department_rounded"
                                    }
                                  },
                                  "color": {
                                    "color": {
                                      "color": "error"
                                    }
                                  },
                                  "size": {
                                    "numberVal": {
                                      "value": 18
                                    }
                                  }
                                },
                                "editorId": "8479ed73-953e-45bc-9e74-5464411d7722"
                              },
                              {
                                "type": "text",
                                "properties": {
                                  "content": {
                                    "slot": {
                                      "name": "difficulty"
                                    }
                                  },
                                  "style": {
                                    "textStyle": {
                                      "styleName": "label_medium"
                                    }
                                  },
                                  "color": {
                                    "color": {
                                      "color": "secondary_text"
                                    }
                                  }
                                },
                                "editorId": "5f4da3db-fc06-46e0-b7fe-d2a1b3a7da96"
                              }
                            ],
                            "editorId": "c2782b66-3652-4232-877d-127223237895"
                          }
                        ],
                        "editorId": "a563ee8a-4a72-459e-aeac-b156d287ff06"
                      }
                    ],
                    "editorId": "9e4949d5-8e38-44f9-a1d7-6c85ac3b1e28"
                  }
                ],
                "editorId": "2dc59f69-a479-4640-b380-894d257372d5"
              }
            ],
            "editorId": "f8309a0c-b9ea-4506-89ca-1467317bb73b"
          }
        ],
        "editorId": "92c2554f-7aa7-4900-adb7-b4ee94dce803"
      }
    },
    {
      "name": "filter_chip",
      "root": {
        "type": "container",
        "properties": {
          "bg": {
            "conditional": {
              "conditionSlot": "selected",
              "trueValue": {
                "color": {
                  "color": "primary"
                }
              },
              "falseValue": {
                "color": {
                  "color": "surface"
                }
              }
            }
          },
          "radius": {
            "radius": {
              "topLeft": 0,
              "topRight": 0,
              "bottomLeft": 0,
              "bottomRight": 0,
              "token": "lg"
            }
          },
          "padding": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "topToken": "sm",
              "rightToken": "lg",
              "bottomToken": "sm",
              "leftToken": "lg"
            }
          },
          "border": {
            "border": {
              "width": 2,
              "color": "divider"
            }
          },
          "shadow": {
            "conditional": {
              "conditionSlot": "selected",
              "trueValue": {
                "stringVal": {
                  "value": "sm"
                }
              },
              "falseValue": {
                "stringVal": {
                  "value": "none"
                }
              }
            }
          }
        },
        "children": [
          {
            "type": "row",
            "properties": {
              "spacing": {
                "stringVal": {
                  "value": "sm"
                }
              },
              "main_size": {
                "stringVal": {
                  "value": "min"
                }
              }
            },
            "children": [
              {
                "type": "icon",
                "properties": {
                  "name": {
                    "slot": {
                      "name": "icon"
                    }
                  },
                  "color": {
                    "conditional": {
                      "conditionSlot": "selected",
                      "trueValue": {
                        "color": {
                          "color": "on_primary"
                        }
                      },
                      "falseValue": {
                        "color": {
                          "color": "primary_text"
                        }
                      }
                    }
                  },
                  "size": {
                    "numberVal": {
                      "value": 18
                    }
                  }
                },
                "editorId": "8e722be7-2fbe-4337-814e-112c45ebea1c"
              },
              {
                "type": "text",
                "properties": {
                  "content": {
                    "slot": {
                      "name": "label"
                    }
                  },
                  "color": {
                    "conditional": {
                      "conditionSlot": "selected",
                      "trueValue": {
                        "color": {
                          "color": "on_primary"
                        }
                      },
                      "falseValue": {
                        "color": {
                          "color": "primary_text"
                        }
                      }
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "label_large"
                    }
                  }
                },
                "editorId": "b71dfbc5-cea8-44d9-b0d6-0c0802002cb7"
              }
            ],
            "editorId": "393ab57c-64bc-4708-a94b-b67a66529279"
          }
        ],
        "editorId": "63fee9a2-6d61-4f88-af5b-260d798dbb68"
      }
    }
  ]
}
```

### 3. Recipe Detail

- Frame ID: `db8aa7eb-43d3-4046-b673-71edbc512fcf`
- Original page prompt: "Full recipe view with description, times, ingredient list, and instructions"
- Follow-up prompts: _None_

#### DslDocument (JSON)

```json
{
  "root": {
    "type": "scaffold",
    "properties": {
      "bg": {
        "color": {
          "color": "background"
        }
      },
      "safe_area": {
        "boolVal": {
          "value": true
        }
      }
    },
    "children": [
      {
        "type": "column",
        "properties": {
          "scroll": {
            "boolVal": {
              "value": true
            }
          },
          "spacing": {
            "stringVal": {
              "value": "lg"
            }
          },
          "padding": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "token": "lg"
            }
          }
        },
        "children": [
          {
            "type": "row",
            "properties": {
              "align": {
                "align": {
                  "named": "space_between"
                }
              }
            },
            "children": [
              {
                "type": "iconbutton",
                "properties": {
                  "name": {
                    "icon": {
                      "name": "arrow_back_rounded"
                    }
                  },
                  "bg": {
                    "color": {
                      "color": "surface"
                    }
                  },
                  "border": {
                    "border": {
                      "width": 2,
                      "color": "divider"
                    }
                  },
                  "radius": {
                    "radius": {
                      "topLeft": 0,
                      "topRight": 0,
                      "bottomLeft": 0,
                      "bottomRight": 0,
                      "token": "md"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  }
                },
                "editorId": "2a1611c2-9c0b-42b7-856c-ecd8af2b5b20"
              },
              {
                "type": "text",
                "properties": {
                  "content": {
                    "stringVal": {
                      "value": "Recipe Details"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "title_large"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  }
                },
                "editorId": "8a730425-e1a1-480b-a9b1-11487e7f6717"
              },
              {
                "type": "iconbutton",
                "properties": {
                  "name": {
                    "icon": {
                      "name": "favorite_rounded"
                    }
                  },
                  "bg": {
                    "color": {
                      "color": "surface"
                    }
                  },
                  "border": {
                    "border": {
                      "width": 2,
                      "color": "divider"
                    }
                  },
                  "radius": {
                    "radius": {
                      "topLeft": 0,
                      "topRight": 0,
                      "bottomLeft": 0,
                      "bottomRight": 0,
                      "token": "md"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary"
                    }
                  }
                },
                "editorId": "6b233790-0cfa-4d3a-ad2a-dfbc3e225f4e"
              }
            ],
            "editorId": "ba3c0c29-3624-421a-94b5-61896e9a239b"
          },
          {
            "type": "container",
            "properties": {
              "height": {
                "px": {
                  "value": 240,
                  "isInfinity": false
                }
              },
              "width": {
                "px": {
                  "value": "Infinity",
                  "isInfinity": true
                }
              },
              "radius": {
                "radius": {
                  "topLeft": 0,
                  "topRight": 0,
                  "bottomLeft": 0,
                  "bottomRight": 0,
                  "token": "xl"
                }
              },
              "border": {
                "border": {
                  "width": 3,
                  "color": "divider"
                }
              },
              "clip": {
                "boolVal": {
                  "value": true
                }
              },
              "shadow": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "stack",
                "properties": {
                  "fit": {
                    "stringVal": {
                      "value": "expand"
                    }
                  }
                },
                "children": [
                  {
                    "type": "image",
                    "properties": {
                      "source_desc": {
                        "imageSource": {
                          "type": "IMAGE_SOURCE_TYPE_DESCRIPTION",
                          "value": "delicious home cooked meal on a colorful plate"
                        }
                      },
                      "fit": {
                        "stringVal": {
                          "value": "cover"
                        }
                      }
                    },
                    "editorId": "9b4cf72b-5833-4afe-9f4a-6f513b5030b0"
                  },
                  {
                    "type": "container",
                    "properties": {
                      "align": {
                        "align": {
                          "named": "bottom_left"
                        }
                      },
                      "padding": {
                        "edgeInsets": {
                          "top": 0,
                          "right": 0,
                          "bottom": 0,
                          "left": 0,
                          "token": "lg"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "container",
                        "properties": {
                          "bg": {
                            "color": {
                              "color": "accent"
                            }
                          },
                          "padding": {
                            "edgeInsets": {
                              "top": 0,
                              "right": 0,
                              "bottom": 0,
                              "left": 0,
                              "topToken": "md",
                              "rightToken": "sm",
                              "bottomToken": "md",
                              "leftToken": "sm"
                            }
                          },
                          "radius": {
                            "radius": {
                              "topLeft": 0,
                              "topRight": 0,
                              "bottomLeft": 0,
                              "bottomRight": 0,
                              "token": "md"
                            }
                          },
                          "border": {
                            "border": {
                              "width": 2,
                              "color": "divider"
                            }
                          }
                        },
                        "children": [
                          {
                            "type": "text",
                            "properties": {
                              "content": {
                                "stringVal": {
                                  "value": "Chef's Choice!"
                                }
                              },
                              "style": {
                                "textStyle": {
                                  "styleName": "label_large"
                                }
                              },
                              "color": {
                                "color": {
                                  "color": "primary_text"
                                }
                              }
                            },
                            "editorId": "1703431b-82fb-4b1d-9920-32785d4284e7"
                          }
                        ],
                        "editorId": "54eb1848-d2bc-4232-884a-b83531dc4e32"
                      }
                    ],
                    "editorId": "e620eeb1-9425-42c9-822b-2fb7d7c0e2db"
                  }
                ],
                "editorId": "d8e9cfd6-e76d-4a9f-adde-071ced88f9ac"
              }
            ],
            "editorId": "e674c6bf-1ee0-4a30-8578-d5e2243e14d0"
          },
          {
            "type": "column",
            "properties": {
              "cross_align": {
                "align": {
                  "named": "start"
                }
              },
              "spacing": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "text",
                "properties": {
                  "content": {
                    "stringVal": {
                      "value": "Sunny Pantry Skillet"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "headline_medium"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  }
                },
                "editorId": "8ed632e0-14cb-4814-99a6-117a6e54b7eb"
              },
              {
                "type": "text",
                "properties": {
                  "content": {
                    "stringVal": {
                      "value": "A simple, hearty dish made with your available ingredients. Perfect for a quick family dinner that's both nutritious and fun to make!"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "body_large"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "secondary_text"
                    }
                  }
                },
                "editorId": "12e11f62-ea77-4485-971d-ee07368ecdec"
              }
            ],
            "editorId": "a81a6009-a97d-40ab-a3ad-7e20d3e69dbe"
          },
          {
            "type": "row",
            "properties": {
              "spacing": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "expanded",
                "children": [
                  {
                    "type": "@time_card",
                    "properties": {
                      "color": {
                        "stringVal": {
                          "value": "secondary"
                        }
                      },
                      "icon": {
                        "stringVal": {
                          "value": "timer_rounded"
                        }
                      },
                      "label": {
                        "stringVal": {
                          "value": "Prep Time"
                        }
                      },
                      "value": {
                        "stringVal": {
                          "value": "10 min"
                        }
                      }
                    },
                    "editorId": "0aa1a58b-d1a8-4a9a-9da7-c8f50c0642af"
                  }
                ],
                "editorId": "39ae4614-b287-4b3a-9e6e-696dd735a264"
              },
              {
                "type": "expanded",
                "children": [
                  {
                    "type": "@time_card",
                    "properties": {
                      "color": {
                        "stringVal": {
                          "value": "success"
                        }
                      },
                      "icon": {
                        "stringVal": {
                          "value": "restaurant_rounded"
                        }
                      },
                      "label": {
                        "stringVal": {
                          "value": "Cook Time"
                        }
                      },
                      "value": {
                        "stringVal": {
                          "value": "20 min"
                        }
                      }
                    },
                    "editorId": "73521d6c-fb24-4dce-9ae0-a37252861850"
                  }
                ],
                "editorId": "bf4e2fa7-5921-4db0-a620-b59fe05433e2"
              }
            ],
            "editorId": "cc45cc31-850d-48ce-9467-8adb41652840"
          },
          {
            "type": "column",
            "properties": {
              "cross_align": {
                "align": {
                  "named": "start"
                }
              },
              "spacing": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "row",
                "properties": {
                  "spacing": {
                    "stringVal": {
                      "value": "sm"
                    }
                  }
                },
                "children": [
                  {
                    "type": "icon",
                    "properties": {
                      "name": {
                        "icon": {
                          "name": "shopping_basket_rounded"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary"
                        }
                      },
                      "size": {
                        "numberVal": {
                          "value": 28
                        }
                      }
                    },
                    "editorId": "86c8db50-78fe-4104-8d7e-f41e21feb90e"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Ingredients"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "title_large"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      }
                    },
                    "editorId": "5b179752-128c-4aca-a932-ce042be23468"
                  }
                ],
                "editorId": "061289fe-c217-4a43-853e-8cf8770806b1"
              },
              {
                "type": "wrap",
                "properties": {
                  "spacing": {
                    "numberVal": {
                      "value": 0
                    }
                  }
                },
                "children": [
                  {
                    "type": "@ingredient_chip",
                    "properties": {
                      "name": {
                        "stringVal": {
                          "value": "2 Large Potatoes"
                        }
                      },
                      "bullet_color": {
                        "stringVal": {
                          "value": "primary"
                        }
                      }
                    },
                    "editorId": "9c7e9bb0-056e-4f31-9c62-474b1df3de3a"
                  },
                  {
                    "type": "@ingredient_chip",
                    "properties": {
                      "name": {
                        "stringVal": {
                          "value": "1 Red Onion"
                        }
                      },
                      "bullet_color": {
                        "stringVal": {
                          "value": "secondary"
                        }
                      }
                    },
                    "editorId": "f3eb4538-5509-4628-af66-3f7a00fa0921"
                  },
                  {
                    "type": "@ingredient_chip",
                    "properties": {
                      "name": {
                        "stringVal": {
                          "value": "3 Fresh Eggs"
                        }
                      },
                      "bullet_color": {
                        "stringVal": {
                          "value": "accent"
                        }
                      }
                    },
                    "editorId": "e3011ff6-dede-4036-bf10-dc7adfa6a468"
                  },
                  {
                    "type": "@ingredient_chip",
                    "properties": {
                      "name": {
                        "stringVal": {
                          "value": "Handful of Spinach"
                        }
                      },
                      "bullet_color": {
                        "stringVal": {
                          "value": "success"
                        }
                      }
                    },
                    "editorId": "cdbce3ca-33eb-4ea5-a5f5-8eff8732eb73"
                  },
                  {
                    "type": "@ingredient_chip",
                    "properties": {
                      "name": {
                        "stringVal": {
                          "value": "Olive Oil"
                        }
                      },
                      "bullet_color": {
                        "stringVal": {
                          "value": "primary_text"
                        }
                      }
                    },
                    "editorId": "06d74596-978d-44bd-b997-a3345a87322a"
                  },
                  {
                    "type": "@ingredient_chip",
                    "properties": {
                      "name": {
                        "stringVal": {
                          "value": "Salt & Pepper"
                        }
                      },
                      "bullet_color": {
                        "stringVal": {
                          "value": "secondary_text"
                        }
                      }
                    },
                    "editorId": "a7d55007-7ca6-42ed-b4ee-5a53a98fe75e"
                  }
                ],
                "editorId": "11d617c8-a2a6-41c5-87eb-79e81c6041f1"
              }
            ],
            "editorId": "cb969d70-afa4-4661-9bf9-6544b16a3e1d"
          },
          {
            "type": "column",
            "properties": {
              "cross_align": {
                "align": {
                  "named": "start"
                }
              },
              "spacing": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "row",
                "properties": {
                  "spacing": {
                    "stringVal": {
                      "value": "sm"
                    }
                  }
                },
                "children": [
                  {
                    "type": "icon",
                    "properties": {
                      "name": {
                        "icon": {
                          "name": "format_list_numbered_rounded"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary"
                        }
                      },
                      "size": {
                        "numberVal": {
                          "value": 28
                        }
                      }
                    },
                    "editorId": "0a852df4-b026-4a9c-b69d-c299ad1a5a82"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Cooking Steps"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "title_large"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      }
                    },
                    "editorId": "f500bb78-46e7-4a33-b860-82dda130b5fb"
                  }
                ],
                "editorId": "cdacdbac-3220-4d3a-aa03-2909ea7ec567"
              },
              {
                "type": "column",
                "properties": {
                  "spacing": {
                    "stringVal": {
                      "value": "lg"
                    }
                  },
                  "cross_align": {
                    "align": {
                      "named": "stretch"
                    }
                  }
                },
                "children": [
                  {
                    "type": "@step_item",
                    "properties": {
                      "number": {
                        "stringVal": {
                          "value": "1"
                        }
                      },
                      "instruction": {
                        "stringVal": {
                          "value": "Wash and dice the potatoes into small, even cubes. Finely chop the onion."
                        }
                      }
                    },
                    "editorId": "68e0adcc-f345-4410-911b-4284d80512f4"
                  },
                  {
                    "type": "@step_item",
                    "properties": {
                      "number": {
                        "stringVal": {
                          "value": "2"
                        }
                      },
                      "instruction": {
                        "stringVal": {
                          "value": "Heat 2 tablespoons of oil in a large skillet. Add potatoes and cook until golden brown and tender (about 12 minutes)."
                        }
                      }
                    },
                    "editorId": "343b4656-6564-4c3d-b483-05e61f72b41f"
                  },
                  {
                    "type": "@step_item",
                    "properties": {
                      "number": {
                        "stringVal": {
                          "value": "3"
                        }
                      },
                      "instruction": {
                        "stringVal": {
                          "value": "Stir in the onions and cook until soft. Add the spinach at the very end until just wilted."
                        }
                      }
                    },
                    "editorId": "57eb11eb-a9cd-4382-874b-4ccbb1bc8560"
                  },
                  {
                    "type": "@step_item",
                    "properties": {
                      "number": {
                        "stringVal": {
                          "value": "4"
                        }
                      },
                      "instruction": {
                        "stringVal": {
                          "value": "Make three small wells in the mixture and crack an egg into each. Cover and cook until eggs are set to your liking."
                        }
                      }
                    },
                    "editorId": "0fe8060d-cb92-4a9b-8e3e-b43af8c6b548"
                  }
                ],
                "editorId": "4976addf-6bde-420c-84cd-b53d4ccc7184"
              }
            ],
            "editorId": "70215450-cd64-4cec-9aa4-6f9ba4385f23"
          },
          {
            "type": "container",
            "properties": {
              "bg": {
                "color": {
                  "color": "primary"
                }
              },
              "radius": {
                "radius": {
                  "topLeft": 0,
                  "topRight": 0,
                  "bottomLeft": 0,
                  "bottomRight": 0,
                  "token": "lg"
                }
              },
              "padding": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "token": "lg"
                }
              },
              "border": {
                "border": {
                  "width": 2,
                  "color": "divider"
                }
              },
              "shadow": {
                "stringVal": {
                  "value": "lg"
                }
              },
              "align_child": {
                "align": {
                  "named": "center"
                }
              }
            },
            "children": [
              {
                "type": "row",
                "properties": {
                  "main_size": {
                    "stringVal": {
                      "value": "min"
                    }
                  },
                  "spacing": {
                    "stringVal": {
                      "value": "md"
                    }
                  }
                },
                "children": [
                  {
                    "type": "icon",
                    "properties": {
                      "name": {
                        "icon": {
                          "name": "celebration_rounded"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "on_primary"
                        }
                      },
                      "size": {
                        "numberVal": {
                          "value": 28
                        }
                      }
                    },
                    "editorId": "9c4a9bc1-ef8c-4be5-8834-265122eaa7d6"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "I Cooked This!"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "title_medium"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "on_primary"
                        }
                      }
                    },
                    "editorId": "d9cf39db-1ffd-4cb7-ab39-4b138ed0e6b1"
                  }
                ],
                "editorId": "f6aa8bc9-d446-4446-991f-a45e00bd37ea"
              }
            ],
            "editorId": "490e7b9a-34f4-4727-aa44-1a8ab222ab90"
          },
          {
            "type": "sizedbox",
            "properties": {
              "height": {
                "stringVal": {
                  "value": "xl"
                }
              }
            },
            "editorId": "426d647d-6629-4075-8075-e3197f7b0956"
          }
        ],
        "editorId": "1ef52926-1611-4bfa-bfd0-dfc7ece9fb3b"
      }
    ],
    "editorId": "1485360d-b0e5-4557-9af0-510a664f37e2"
  },
  "components": [
    {
      "name": "time_card",
      "root": {
        "type": "container",
        "properties": {
          "bg": {
            "slot": {
              "name": "color"
            }
          },
          "radius": {
            "radius": {
              "topLeft": 0,
              "topRight": 0,
              "bottomLeft": 0,
              "bottomRight": 0,
              "token": "lg"
            }
          },
          "padding": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "token": "md"
            }
          },
          "border": {
            "border": {
              "width": 2,
              "color": "divider"
            }
          },
          "shadow": {
            "stringVal": {
              "value": "sm"
            }
          }
        },
        "children": [
          {
            "type": "column",
            "properties": {
              "spacing": {
                "stringVal": {
                  "value": "xs"
                }
              }
            },
            "children": [
              {
                "type": "icon",
                "properties": {
                  "name": {
                    "slot": {
                      "name": "icon"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  },
                  "size": {
                    "numberVal": {
                      "value": 24
                    }
                  }
                },
                "editorId": "50f16fc7-d70b-4592-8308-a8474d6f9902"
              },
              {
                "type": "text",
                "properties": {
                  "content": {
                    "slot": {
                      "name": "label"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "label_small"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  }
                },
                "editorId": "129e58ba-9f0c-4617-b4db-6c61c09fab9c"
              },
              {
                "type": "text",
                "properties": {
                  "content": {
                    "slot": {
                      "name": "value"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "title_medium"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  }
                },
                "editorId": "521d9ef1-d401-4ce6-9dea-176b061d751b"
              }
            ],
            "editorId": "040df6ee-198f-4d0e-a2eb-6d9485117df3"
          }
        ],
        "editorId": "560df5e2-25ea-4147-bd1f-2c01807eb9b1"
      }
    },
    {
      "name": "ingredient_chip",
      "root": {
        "type": "container",
        "properties": {
          "bg": {
            "color": {
              "color": "surface"
            }
          },
          "radius": {
            "radius": {
              "topLeft": 0,
              "topRight": 0,
              "bottomLeft": 0,
              "bottomRight": 0,
              "token": "full"
            }
          },
          "padding": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "topToken": "md",
              "rightToken": "sm",
              "bottomToken": "md",
              "leftToken": "sm"
            }
          },
          "border": {
            "border": {
              "width": 2,
              "color": "divider"
            }
          },
          "margin": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "rightToken": "sm",
              "bottomToken": "sm"
            }
          }
        },
        "children": [
          {
            "type": "row",
            "properties": {
              "spacing": {
                "stringVal": {
                  "value": "sm"
                }
              },
              "main_size": {
                "stringVal": {
                  "value": "min"
                }
              }
            },
            "children": [
              {
                "type": "container",
                "properties": {
                  "width": {
                    "px": {
                      "value": 12,
                      "isInfinity": false
                    }
                  },
                  "height": {
                    "px": {
                      "value": 12,
                      "isInfinity": false
                    }
                  },
                  "bg": {
                    "slot": {
                      "name": "bullet_color"
                    }
                  },
                  "radius": {
                    "radius": {
                      "topLeft": 0,
                      "topRight": 0,
                      "bottomLeft": 0,
                      "bottomRight": 0,
                      "token": "full"
                    }
                  },
                  "border": {
                    "border": {
                      "width": 1,
                      "color": "divider"
                    }
                  }
                },
                "editorId": "159e6fc7-905c-4b7c-a643-d35f4b7b7a51"
              },
              {
                "type": "text",
                "properties": {
                  "content": {
                    "slot": {
                      "name": "name"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "body_medium"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  }
                },
                "editorId": "febc6ea8-1de4-4e78-8416-79a481a305a7"
              }
            ],
            "editorId": "edb20095-8ab9-463b-984b-3b4557d86dd2"
          }
        ],
        "editorId": "af6f6ad4-f831-43c1-add8-da19348de974"
      }
    },
    {
      "name": "step_item",
      "root": {
        "type": "row",
        "properties": {
          "cross_align": {
            "align": {
              "named": "start"
            }
          },
          "spacing": {
            "stringVal": {
              "value": "md"
            }
          }
        },
        "children": [
          {
            "type": "container",
            "properties": {
              "width": {
                "px": {
                  "value": 40,
                  "isInfinity": false
                }
              },
              "height": {
                "px": {
                  "value": 40,
                  "isInfinity": false
                }
              },
              "bg": {
                "color": {
                  "color": "accent"
                }
              },
              "radius": {
                "radius": {
                  "topLeft": 0,
                  "topRight": 0,
                  "bottomLeft": 0,
                  "bottomRight": 0,
                  "token": "full"
                }
              },
              "border": {
                "border": {
                  "width": 2,
                  "color": "divider"
                }
              },
              "align_child": {
                "align": {
                  "named": "center"
                }
              },
              "shadow": {
                "stringVal": {
                  "value": "sm"
                }
              }
            },
            "children": [
              {
                "type": "text",
                "properties": {
                  "content": {
                    "slot": {
                      "name": "number"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "title_medium"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  }
                },
                "editorId": "59123d28-2114-43c2-843b-e72a9bb83bf5"
              }
            ],
            "editorId": "1a4902e0-7614-444e-8e12-fe309fe17cb0"
          },
          {
            "type": "expanded",
            "children": [
              {
                "type": "container",
                "properties": {
                  "bg": {
                    "color": {
                      "color": "surface"
                    }
                  },
                  "radius": {
                    "radius": {
                      "topLeft": 0,
                      "topRight": 0,
                      "bottomLeft": 0,
                      "bottomRight": 0,
                      "token": "lg"
                    }
                  },
                  "padding": {
                    "edgeInsets": {
                      "top": 0,
                      "right": 0,
                      "bottom": 0,
                      "left": 0,
                      "token": "lg"
                    }
                  },
                  "border": {
                    "border": {
                      "width": 2,
                      "color": "divider"
                    }
                  }
                },
                "children": [
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "slot": {
                          "name": "instruction"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "body_medium"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      }
                    },
                    "editorId": "2fa91c5b-1e4e-4541-8781-d9111f000467"
                  }
                ],
                "editorId": "f139e555-d767-4183-b983-d51e3f05795a"
              }
            ],
            "editorId": "fbbd6336-6297-4f41-8215-bfc1feefff43"
          }
        ],
        "editorId": "d5922bcb-6e8e-441c-b62b-b9623345f8a3"
      }
    }
  ]
}
```

### 4. Saved Recipes

- Frame ID: `8a9742eb-6be3-4323-aac4-ae29a97a9d87`
- Original page prompt: "A collection of the user's favorite and previously cooked dishes"
- Follow-up prompts: _None_

#### DslDocument (JSON)

```json
{
  "root": {
    "type": "scaffold",
    "properties": {
      "bg": {
        "color": {
          "color": "background"
        }
      },
      "safe_area": {
        "boolVal": {
          "value": true
        }
      }
    },
    "children": [
      {
        "type": "column",
        "properties": {
          "scroll": {
            "boolVal": {
              "value": true
            }
          },
          "spacing": {
            "numberVal": {
              "value": 0
            }
          }
        },
        "children": [
          {
            "type": "container",
            "properties": {
              "padding": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "token": "lg"
                }
              },
              "border": {
                "borderSided": {
                  "side": "bottom",
                  "width": 3,
                  "color": "divider"
                }
              },
              "bg": {
                "color": {
                  "color": "surface"
                }
              }
            },
            "children": [
              {
                "type": "row",
                "properties": {
                  "align": {
                    "align": {
                      "named": "space_between"
                    }
                  }
                },
                "children": [
                  {
                    "type": "column",
                    "properties": {
                      "cross_align": {
                        "align": {
                          "named": "start"
                        }
                      },
                      "spacing": {
                        "stringVal": {
                          "value": "xs"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "text",
                        "properties": {
                          "content": {
                            "stringVal": {
                              "value": "Your Kitchen"
                            }
                          },
                          "style": {
                            "textStyle": {
                              "styleName": "label_medium"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "secondary_text"
                            }
                          }
                        },
                        "editorId": "e20210be-d4b4-44e4-9a31-dfaf797dc582"
                      },
                      {
                        "type": "text",
                        "properties": {
                          "content": {
                            "stringVal": {
                              "value": "Saved Recipes"
                            }
                          },
                          "style": {
                            "textStyle": {
                              "styleName": "headline_medium"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary_text"
                            }
                          },
                          "font_weight": {
                            "numberVal": {
                              "value": 900
                            }
                          }
                        },
                        "editorId": "e9134e92-b99c-456e-b814-f276314a5e29"
                      }
                    ],
                    "editorId": "5a06ab65-b997-4e3e-b7ff-a6598a59c294"
                  },
                  {
                    "type": "container",
                    "properties": {
                      "width": {
                        "px": {
                          "value": 48,
                          "isInfinity": false
                        }
                      },
                      "height": {
                        "px": {
                          "value": 48,
                          "isInfinity": false
                        }
                      },
                      "bg": {
                        "color": {
                          "color": "secondary"
                        }
                      },
                      "radius": {
                        "radius": {
                          "topLeft": 0,
                          "topRight": 0,
                          "bottomLeft": 0,
                          "bottomRight": 0,
                          "token": "lg"
                        }
                      },
                      "border": {
                        "border": {
                          "width": 2,
                          "color": "divider"
                        }
                      },
                      "align_child": {
                        "align": {
                          "named": "center"
                        }
                      },
                      "shadow": {
                        "stringVal": {
                          "value": "sm"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "icon",
                        "properties": {
                          "name": {
                            "icon": {
                              "name": "search_rounded"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary_text"
                            }
                          },
                          "size": {
                            "numberVal": {
                              "value": 28
                            }
                          }
                        },
                        "editorId": "e7451441-e767-4ad0-b85f-79f832c89456"
                      }
                    ],
                    "editorId": "b4d82347-f0d6-4d07-876d-83355cdd011b"
                  }
                ],
                "editorId": "15da410f-4f5a-4383-8e93-5e58bb8c8a5d"
              }
            ],
            "editorId": "e1fc55f5-d27e-485f-aa84-9f3d02c9c2be"
          },
          {
            "type": "container",
            "properties": {
              "padding": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "topToken": "lg",
                  "bottomToken": "lg",
                  "leftToken": "lg"
                }
              }
            },
            "children": [
              {
                "type": "row",
                "properties": {
                  "scroll": {
                    "boolVal": {
                      "value": true
                    }
                  },
                  "spacing": {
                    "numberVal": {
                      "value": 0
                    }
                  }
                },
                "children": [
                  {
                    "type": "@filter_chip",
                    "properties": {
                      "label": {
                        "stringVal": {
                          "value": "All Dishes"
                        }
                      },
                      "selected": {
                        "boolVal": {
                          "value": true
                        }
                      }
                    },
                    "editorId": "ab915519-990c-40c2-b5b0-8280644f06c1"
                  },
                  {
                    "type": "@filter_chip",
                    "properties": {
                      "label": {
                        "stringVal": {
                          "value": "Breakfast"
                        }
                      },
                      "selected": {
                        "boolVal": {
                          "value": false
                        }
                      }
                    },
                    "editorId": "f02c0623-5ec4-4d14-8766-0885e8e8392b"
                  },
                  {
                    "type": "@filter_chip",
                    "properties": {
                      "label": {
                        "stringVal": {
                          "value": "Quick Lunch"
                        }
                      },
                      "selected": {
                        "boolVal": {
                          "value": false
                        }
                      }
                    },
                    "editorId": "662645a9-7543-4b43-8084-8fc6fe7ae51b"
                  },
                  {
                    "type": "@filter_chip",
                    "properties": {
                      "label": {
                        "stringVal": {
                          "value": "Dinner"
                        }
                      },
                      "selected": {
                        "boolVal": {
                          "value": false
                        }
                      }
                    },
                    "editorId": "62c7581b-3392-4c8a-b8b6-b26d425a231c"
                  },
                  {
                    "type": "@filter_chip",
                    "properties": {
                      "label": {
                        "stringVal": {
                          "value": "Desserts"
                        }
                      },
                      "selected": {
                        "boolVal": {
                          "value": false
                        }
                      }
                    },
                    "editorId": "2c2abbd0-d807-4376-826a-7bd2411a43fe"
                  }
                ],
                "editorId": "2f2db4ea-12f4-46a3-a720-f8f4cca18302"
              }
            ],
            "editorId": "803233ba-8111-4c67-b6db-d599431c0916"
          },
          {
            "type": "container",
            "properties": {
              "margin": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "rightToken": "lg",
                  "bottomToken": "lg",
                  "leftToken": "lg"
                }
              },
              "padding": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "token": "lg"
                }
              },
              "bg": {
                "color": {
                  "color": "secondary"
                }
              },
              "radius": {
                "radius": {
                  "topLeft": 0,
                  "topRight": 0,
                  "bottomLeft": 0,
                  "bottomRight": 0,
                  "token": "xl"
                }
              },
              "border": {
                "border": {
                  "width": 3,
                  "color": "divider"
                }
              },
              "shadow": {
                "stringVal": {
                  "value": "sm"
                }
              }
            },
            "children": [
              {
                "type": "row",
                "properties": {
                  "align": {
                    "align": {
                      "named": "space_around"
                    }
                  }
                },
                "children": [
                  {
                    "type": "column",
                    "properties": {
                      "spacing": {
                        "stringVal": {
                          "value": "xs"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "text",
                        "properties": {
                          "content": {
                            "stringVal": {
                              "value": "12"
                            }
                          },
                          "style": {
                            "textStyle": {
                              "styleName": "headline_small"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary_text"
                            }
                          },
                          "font_weight": {
                            "numberVal": {
                              "value": 900
                            }
                          }
                        },
                        "editorId": "fc7b28c2-e5d2-41a9-ada5-13acd6c32ed4"
                      },
                      {
                        "type": "text",
                        "properties": {
                          "content": {
                            "stringVal": {
                              "value": "Cooked"
                            }
                          },
                          "style": {
                            "textStyle": {
                              "styleName": "label_small"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary_text"
                            }
                          }
                        },
                        "editorId": "4d1dc1fc-de4c-457d-ba24-e2e026ba88bb"
                      }
                    ],
                    "editorId": "a8dd8e8c-fd0f-493b-98fe-e85a6233940c"
                  },
                  {
                    "type": "container",
                    "properties": {
                      "width": {
                        "px": {
                          "value": 2,
                          "isInfinity": false
                        }
                      },
                      "height": {
                        "px": {
                          "value": 30,
                          "isInfinity": false
                        }
                      },
                      "bg": {
                        "color": {
                          "color": "divider"
                        }
                      }
                    },
                    "editorId": "e9b15d69-c764-4373-8200-c6737a163188"
                  },
                  {
                    "type": "column",
                    "properties": {
                      "spacing": {
                        "stringVal": {
                          "value": "xs"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "text",
                        "properties": {
                          "content": {
                            "stringVal": {
                              "value": "24"
                            }
                          },
                          "style": {
                            "textStyle": {
                              "styleName": "headline_small"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary_text"
                            }
                          },
                          "font_weight": {
                            "numberVal": {
                              "value": 900
                            }
                          }
                        },
                        "editorId": "17b01804-52bf-4fe3-8443-185670d1ebd0"
                      },
                      {
                        "type": "text",
                        "properties": {
                          "content": {
                            "stringVal": {
                              "value": "Saved"
                            }
                          },
                          "style": {
                            "textStyle": {
                              "styleName": "label_small"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary_text"
                            }
                          }
                        },
                        "editorId": "f1cb188d-516d-4a67-a391-7048ab95b0f9"
                      }
                    ],
                    "editorId": "bd961442-e116-485d-84f9-fed838c71d1c"
                  },
                  {
                    "type": "container",
                    "properties": {
                      "width": {
                        "px": {
                          "value": 2,
                          "isInfinity": false
                        }
                      },
                      "height": {
                        "px": {
                          "value": 30,
                          "isInfinity": false
                        }
                      },
                      "bg": {
                        "color": {
                          "color": "divider"
                        }
                      }
                    },
                    "editorId": "0d73991e-9262-4d20-a2d9-89cac260cbe7"
                  },
                  {
                    "type": "column",
                    "properties": {
                      "spacing": {
                        "stringVal": {
                          "value": "xs"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "text",
                        "properties": {
                          "content": {
                            "stringVal": {
                              "value": "4.8"
                            }
                          },
                          "style": {
                            "textStyle": {
                              "styleName": "headline_small"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary_text"
                            }
                          },
                          "font_weight": {
                            "numberVal": {
                              "value": 900
                            }
                          }
                        },
                        "editorId": "4908190b-e50c-44e8-8e87-5487e13ea4ed"
                      },
                      {
                        "type": "text",
                        "properties": {
                          "content": {
                            "stringVal": {
                              "value": "Avg Rating"
                            }
                          },
                          "style": {
                            "textStyle": {
                              "styleName": "label_small"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary_text"
                            }
                          }
                        },
                        "editorId": "0740e9eb-cd59-4101-871f-6ff40be8946e"
                      }
                    ],
                    "editorId": "3529a659-cc99-475c-b762-082a541223ea"
                  }
                ],
                "editorId": "d9a9769e-aa37-46d1-be12-0594eff2f6fe"
              }
            ],
            "editorId": "7de8e144-f067-498d-a41f-7335c7f0eb59"
          },
          {
            "type": "column",
            "properties": {
              "padding": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "token": "lg"
                }
              },
              "spacing": {
                "numberVal": {
                  "value": 0
                }
              }
            },
            "children": [
              {
                "type": "@recipe_card",
                "properties": {
                  "title": {
                    "stringVal": {
                      "value": "Creamy Garlic Pasta"
                    }
                  },
                  "img_desc": {
                    "stringVal": {
                      "value": "plate of creamy pasta with herbs"
                    }
                  },
                  "category": {
                    "stringVal": {
                      "value": "Italian"
                    }
                  },
                  "description": {
                    "stringVal": {
                      "value": "A 15-minute pantry staple using just garlic, cream, and parmesan."
                    }
                  },
                  "time": {
                    "stringVal": {
                      "value": "15 min"
                    }
                  },
                  "difficulty": {
                    "stringVal": {
                      "value": "Easy"
                    }
                  }
                },
                "editorId": "ad8f776f-9e86-4417-845a-1f54e09ea3d0"
              },
              {
                "type": "@recipe_card",
                "properties": {
                  "title": {
                    "stringVal": {
                      "value": "Spicy Chickpea Wrap"
                    }
                  },
                  "img_desc": {
                    "stringVal": {
                      "value": "healthy veggie wrap with chickpeas"
                    }
                  },
                  "category": {
                    "stringVal": {
                      "value": "Vegan"
                    }
                  },
                  "description": {
                    "stringVal": {
                      "value": "Protein-packed wraps with a zesty tahini dressing and fresh greens."
                    }
                  },
                  "time": {
                    "stringVal": {
                      "value": "10 min"
                    }
                  },
                  "difficulty": {
                    "stringVal": {
                      "value": "Medium"
                    }
                  }
                },
                "editorId": "c52e9863-cf00-4b07-83f9-ac280b47c4f0"
              },
              {
                "type": "@recipe_card",
                "properties": {
                  "title": {
                    "stringVal": {
                      "value": "Honey Glazed Salmon"
                    }
                  },
                  "img_desc": {
                    "stringVal": {
                      "value": "grilled salmon with asparagus"
                    }
                  },
                  "category": {
                    "stringVal": {
                      "value": "Dinner"
                    }
                  },
                  "description": {
                    "stringVal": {
                      "value": "Perfectly seared salmon with a sweet and savory glaze."
                    }
                  },
                  "time": {
                    "stringVal": {
                      "value": "25 min"
                    }
                  },
                  "difficulty": {
                    "stringVal": {
                      "value": "Medium"
                    }
                  }
                },
                "editorId": "71e925c6-c92b-4b1b-8cc3-25fa4c86be66"
              },
              {
                "type": "@recipe_card",
                "properties": {
                  "title": {
                    "stringVal": {
                      "value": "Berry Smoothie Bowl"
                    }
                  },
                  "img_desc": {
                    "stringVal": {
                      "value": "colorful smoothie bowl with fruit"
                    }
                  },
                  "category": {
                    "stringVal": {
                      "value": "Breakfast"
                    }
                  },
                  "description": {
                    "stringVal": {
                      "value": "Antioxidant-rich breakfast topped with granola and fresh berries."
                    }
                  },
                  "time": {
                    "stringVal": {
                      "value": "5 min"
                    }
                  },
                  "difficulty": {
                    "stringVal": {
                      "value": "Easy"
                    }
                  }
                },
                "editorId": "2a180e3f-8fff-490a-b9ca-6a72b5f1c7a9"
              }
            ],
            "editorId": "fb0e0081-d91d-4616-9bf0-84d293c1f289"
          },
          {
            "type": "container",
            "properties": {
              "margin": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "token": "lg"
                }
              },
              "padding": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "token": "xl"
                }
              },
              "radius": {
                "radius": {
                  "topLeft": 0,
                  "topRight": 0,
                  "bottomLeft": 0,
                  "bottomRight": 0,
                  "token": "xl"
                }
              },
              "border": {
                "border": {
                  "width": 2,
                  "color": "divider"
                }
              },
              "bg": {
                "color": {
                  "color": "surface"
                }
              },
              "border_style": {
                "stringVal": {
                  "value": "dashed"
                }
              }
            },
            "children": [
              {
                "type": "column",
                "properties": {
                  "spacing": {
                    "stringVal": {
                      "value": "md"
                    }
                  }
                },
                "children": [
                  {
                    "type": "icon",
                    "properties": {
                      "name": {
                        "icon": {
                          "name": "add_circle_outline_rounded"
                        }
                      },
                      "size": {
                        "numberVal": {
                          "value": 48
                        }
                      },
                      "color": {
                        "color": {
                          "color": "hint"
                        }
                      }
                    },
                    "editorId": "2cfad274-c51e-4516-b21c-0a3eeffe2694"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Looking for more?"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "title_medium"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      }
                    },
                    "editorId": "f5511a71-3ea1-4176-af5b-0e186d3d1aa7"
                  },
                  {
                    "type": "button",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Find New Recipes"
                        }
                      },
                      "bg": {
                        "color": {
                          "color": "primary"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "on_primary"
                        }
                      },
                      "radius": {
                        "radius": {
                          "topLeft": 0,
                          "topRight": 0,
                          "bottomLeft": 0,
                          "bottomRight": 0,
                          "token": "md"
                        }
                      },
                      "font_size": {
                        "numberVal": {
                          "value": 14
                        }
                      },
                      "content_padding": {
                        "edgeInsets": {
                          "top": 0,
                          "right": 0,
                          "bottom": 0,
                          "left": 0,
                          "topToken": "lg",
                          "rightToken": "md",
                          "bottomToken": "lg",
                          "leftToken": "md"
                        }
                      }
                    },
                    "editorId": "21e9c50e-2d23-4b21-9f8a-0413097d8b32"
                  }
                ],
                "editorId": "e92500a1-0946-4802-a016-911435ce853c"
              }
            ],
            "editorId": "6c03ef4b-9a1b-49db-8638-5ae654f03514"
          },
          {
            "type": "sizedbox",
            "properties": {
              "height": {
                "stringVal": {
                  "value": "xl"
                }
              }
            },
            "editorId": "d5ff2b96-d680-414f-a65b-dd9768290be9"
          }
        ],
        "editorId": "93bc1ad5-7a79-4aac-a988-be01b7b40c7f"
      },
      {
        "type": "fab",
        "properties": {
          "icon": {
            "icon": {
              "name": "add_rounded"
            }
          },
          "label": {
            "stringVal": {
              "value": "Add Recipe"
            }
          },
          "bg": {
            "color": {
              "color": "primary"
            }
          },
          "color": {
            "color": {
              "color": "on_primary"
            }
          },
          "radius": {
            "radius": {
              "topLeft": 0,
              "topRight": 0,
              "bottomLeft": 0,
              "bottomRight": 0,
              "token": "lg"
            }
          }
        },
        "editorId": "ffac2570-4120-4e4f-a8a3-30e9864e09af"
      }
    ],
    "editorId": "fac7d85a-27eb-48f4-99e5-eb9449816eb4"
  },
  "components": [
    {
      "name": "recipe_card",
      "root": {
        "type": "container",
        "properties": {
          "bg": {
            "color": {
              "color": "surface"
            }
          },
          "radius": {
            "radius": {
              "topLeft": 0,
              "topRight": 0,
              "bottomLeft": 0,
              "bottomRight": 0,
              "token": "xl"
            }
          },
          "border": {
            "border": {
              "width": 3,
              "color": "divider"
            }
          },
          "margin": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "bottomToken": "lg"
            }
          },
          "clip": {
            "boolVal": {
              "value": true
            }
          },
          "shadow": {
            "stringVal": {
              "value": "md"
            }
          }
        },
        "children": [
          {
            "type": "column",
            "properties": {
              "cross_align": {
                "align": {
                  "named": "stretch"
                }
              }
            },
            "children": [
              {
                "type": "stack",
                "properties": {
                  "height": {
                    "px": {
                      "value": 160,
                      "isInfinity": false
                    }
                  }
                },
                "children": [
                  {
                    "type": "image",
                    "properties": {
                      "source_desc": {
                        "slot": {
                          "name": "img_desc"
                        }
                      },
                      "fit": {
                        "stringVal": {
                          "value": "cover"
                        }
                      },
                      "width": {
                        "px": {
                          "value": "Infinity",
                          "isInfinity": true
                        }
                      },
                      "height": {
                        "px": {
                          "value": 160,
                          "isInfinity": false
                        }
                      }
                    },
                    "editorId": "85800b0e-a12d-4064-be85-8b3d66b81f8d"
                  },
                  {
                    "type": "container",
                    "properties": {
                      "align": {
                        "align": {
                          "named": "top_right"
                        }
                      },
                      "padding": {
                        "edgeInsets": {
                          "top": 0,
                          "right": 0,
                          "bottom": 0,
                          "left": 0,
                          "token": "md"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "iconbutton",
                        "properties": {
                          "name": {
                            "icon": {
                              "name": "favorite_rounded"
                            }
                          },
                          "bg": {
                            "color": {
                              "color": "surface"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "error"
                            }
                          },
                          "radius": {
                            "radius": {
                              "topLeft": 0,
                              "topRight": 0,
                              "bottomLeft": 0,
                              "bottomRight": 0,
                              "token": "md"
                            }
                          },
                          "border": {
                            "border": {
                              "width": 2,
                              "color": "divider"
                            }
                          },
                          "size": {
                            "numberVal": {
                              "value": 20
                            }
                          }
                        },
                        "editorId": "9f4d41d3-6951-4e81-85c2-e1b478f1b621"
                      }
                    ],
                    "editorId": "b84c32e5-c59d-48d4-86b9-bcc51ebc6ee0"
                  },
                  {
                    "type": "container",
                    "properties": {
                      "align": {
                        "align": {
                          "named": "bottom_left"
                        }
                      },
                      "padding": {
                        "edgeInsets": {
                          "top": 0,
                          "right": 0,
                          "bottom": 0,
                          "left": 0,
                          "token": "md"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "container",
                        "properties": {
                          "bg": {
                            "color": {
                              "color": "accent"
                            }
                          },
                          "radius": {
                            "radius": {
                              "topLeft": 0,
                              "topRight": 0,
                              "bottomLeft": 0,
                              "bottomRight": 0,
                              "token": "md"
                            }
                          },
                          "border": {
                            "border": {
                              "width": 2,
                              "color": "divider"
                            }
                          },
                          "padding": {
                            "edgeInsets": {
                              "top": 0,
                              "right": 0,
                              "bottom": 0,
                              "left": 0,
                              "topToken": "xs",
                              "rightToken": "sm",
                              "bottomToken": "xs",
                              "leftToken": "sm"
                            }
                          }
                        },
                        "children": [
                          {
                            "type": "text",
                            "properties": {
                              "content": {
                                "slot": {
                                  "name": "category"
                                }
                              },
                              "style": {
                                "textStyle": {
                                  "styleName": "label_small"
                                }
                              },
                              "color": {
                                "color": {
                                  "color": "primary_text"
                                }
                              },
                              "font_weight": {
                                "stringVal": {
                                  "value": "bold"
                                }
                              }
                            },
                            "editorId": "c41adca7-93c2-4cc1-92ed-0bee5d929b5e"
                          }
                        ],
                        "editorId": "528aba51-f006-4647-84c5-382a0d5a6b56"
                      }
                    ],
                    "editorId": "a5224855-d998-4048-af33-c68cf23ba337"
                  }
                ],
                "editorId": "f7ea3c22-2b7d-4d44-a91e-ec87e9c7b6a0"
              },
              {
                "type": "column",
                "properties": {
                  "padding": {
                    "edgeInsets": {
                      "top": 0,
                      "right": 0,
                      "bottom": 0,
                      "left": 0,
                      "token": "lg"
                    }
                  },
                  "spacing": {
                    "stringVal": {
                      "value": "sm"
                    }
                  },
                  "cross_align": {
                    "align": {
                      "named": "start"
                    }
                  }
                },
                "children": [
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "slot": {
                          "name": "title"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "title_large"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      },
                      "max_lines": {
                        "numberVal": {
                          "value": 1
                        }
                      },
                      "overflow": {
                        "stringVal": {
                          "value": "ellipsis"
                        }
                      }
                    },
                    "editorId": "7d6e2df6-9a51-41c5-8c8d-a78bd83015eb"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "slot": {
                          "name": "description"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "body_small"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "secondary_text"
                        }
                      },
                      "max_lines": {
                        "numberVal": {
                          "value": 2
                        }
                      },
                      "overflow": {
                        "stringVal": {
                          "value": "ellipsis"
                        }
                      }
                    },
                    "editorId": "df9d5c6c-d2d1-476b-8393-079fef261b6e"
                  },
                  {
                    "type": "divider",
                    "properties": {
                      "color": {
                        "color": {
                          "color": "divider"
                        }
                      },
                      "thickness": {
                        "numberVal": {
                          "value": 2
                        }
                      },
                      "margin": {
                        "edgeInsets": {
                          "top": 0,
                          "right": 0,
                          "bottom": 0,
                          "left": 0,
                          "topToken": "sm",
                          "bottomToken": "sm"
                        }
                      }
                    },
                    "editorId": "3e1ade5d-8b00-4f55-a0da-486d10fcabe7"
                  },
                  {
                    "type": "row",
                    "properties": {
                      "align": {
                        "align": {
                          "named": "space_between"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "row",
                        "properties": {
                          "spacing": {
                            "stringVal": {
                              "value": "xs"
                            }
                          }
                        },
                        "children": [
                          {
                            "type": "icon",
                            "properties": {
                              "name": {
                                "icon": {
                                  "name": "schedule_rounded"
                                }
                              },
                              "size": {
                                "numberVal": {
                                  "value": 16
                                }
                              },
                              "color": {
                                "color": {
                                  "color": "primary"
                                }
                              }
                            },
                            "editorId": "ddd76323-571b-47ef-81c1-3a4f349f2f4b"
                          },
                          {
                            "type": "text",
                            "properties": {
                              "content": {
                                "slot": {
                                  "name": "time"
                                }
                              },
                              "style": {
                                "textStyle": {
                                  "styleName": "label_medium"
                                }
                              },
                              "color": {
                                "color": {
                                  "color": "primary_text"
                                }
                              }
                            },
                            "editorId": "2fb9c61b-7918-4aa5-8a78-5fd5fcfd9c85"
                          }
                        ],
                        "editorId": "58642230-a6fd-45b6-ae0c-83242e5bfeff"
                      },
                      {
                        "type": "row",
                        "properties": {
                          "spacing": {
                            "stringVal": {
                              "value": "xs"
                            }
                          }
                        },
                        "children": [
                          {
                            "type": "icon",
                            "properties": {
                              "name": {
                                "icon": {
                                  "name": "local_fire_department_rounded"
                                }
                              },
                              "size": {
                                "numberVal": {
                                  "value": 16
                                }
                              },
                              "color": {
                                "color": {
                                  "color": "secondary"
                                }
                              }
                            },
                            "editorId": "42051718-4bbe-4ef9-bff1-ab5db6ef8c6d"
                          },
                          {
                            "type": "text",
                            "properties": {
                              "content": {
                                "slot": {
                                  "name": "difficulty"
                                }
                              },
                              "style": {
                                "textStyle": {
                                  "styleName": "label_medium"
                                }
                              },
                              "color": {
                                "color": {
                                  "color": "primary_text"
                                }
                              }
                            },
                            "editorId": "141c521a-76f4-4bc7-a162-060c6bbf7749"
                          }
                        ],
                        "editorId": "31ffd0dc-73f5-4981-a22b-31dd5558183e"
                      }
                    ],
                    "editorId": "d79322bd-0cd7-4681-b272-30aacfa85ab7"
                  }
                ],
                "editorId": "88fea290-ac02-4e17-a1ff-ea30348c5a29"
              }
            ],
            "editorId": "c767b7ce-82d2-4612-b6fa-596460c5e225"
          }
        ],
        "editorId": "e1583a70-183b-4162-8bd5-0cc17dd764a4"
      }
    },
    {
      "name": "filter_chip",
      "root": {
        "type": "container",
        "properties": {
          "bg": {
            "conditional": {
              "conditionSlot": "selected",
              "trueValue": {
                "color": {
                  "color": "primary"
                }
              },
              "falseValue": {
                "color": {
                  "color": "surface"
                }
              }
            }
          },
          "radius": {
            "radius": {
              "topLeft": 0,
              "topRight": 0,
              "bottomLeft": 0,
              "bottomRight": 0,
              "token": "lg"
            }
          },
          "border": {
            "border": {
              "width": 2,
              "color": "divider"
            }
          },
          "padding": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "topToken": "sm",
              "rightToken": "lg",
              "bottomToken": "sm",
              "leftToken": "lg"
            }
          },
          "margin": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "rightToken": "md"
            }
          }
        },
        "children": [
          {
            "type": "text",
            "properties": {
              "content": {
                "slot": {
                  "name": "label"
                }
              },
              "color": {
                "conditional": {
                  "conditionSlot": "selected",
                  "trueValue": {
                    "color": {
                      "color": "on_primary"
                    }
                  },
                  "falseValue": {
                    "color": {
                      "color": "primary_text"
                    }
                  }
                }
              },
              "font_weight": {
                "stringVal": {
                  "value": "bold"
                }
              },
              "style": {
                "textStyle": {
                  "styleName": "label_large"
                }
              }
            },
            "editorId": "5b48d069-6eba-4bcd-ba97-496e2ee4e28b"
          }
        ],
        "editorId": "32848d20-5ed8-428c-acb5-6f41c31491b0"
      }
    }
  ]
}
```

### 5. Chef Profile

- Frame ID: `6bc3400d-b350-44c9-bd69-1bce3ae37fbf`
- Original page prompt: "User profile with dietary preferences and cooking skill level"
- Follow-up prompts: _None_

#### DslDocument (JSON)

```json
{
  "root": {
    "type": "scaffold",
    "properties": {
      "bg": {
        "color": {
          "color": "background"
        }
      },
      "safe_area": {
        "boolVal": {
          "value": true
        }
      }
    },
    "children": [
      {
        "type": "column",
        "properties": {
          "scroll": {
            "boolVal": {
              "value": true
            }
          },
          "spacing": {
            "stringVal": {
              "value": "lg"
            }
          },
          "padding": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "token": "lg"
            }
          }
        },
        "children": [
          {
            "type": "row",
            "properties": {
              "align": {
                "align": {
                  "named": "space_between"
                }
              }
            },
            "children": [
              {
                "type": "iconbutton",
                "properties": {
                  "name": {
                    "icon": {
                      "name": "arrow_back_rounded"
                    }
                  },
                  "bg": {
                    "color": {
                      "color": "surface"
                    }
                  },
                  "border": {
                    "border": {
                      "width": 2,
                      "color": "divider"
                    }
                  },
                  "radius": {
                    "radius": {
                      "topLeft": 0,
                      "topRight": 0,
                      "bottomLeft": 0,
                      "bottomRight": 0,
                      "token": "md"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  }
                },
                "editorId": "a35c56fd-1a0b-4b37-b66e-43d9d28bc7a8"
              },
              {
                "type": "text",
                "properties": {
                  "content": {
                    "stringVal": {
                      "value": "Chef Profile"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "title_large"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  },
                  "font_weight": {
                    "numberVal": {
                      "value": 800
                    }
                  }
                },
                "editorId": "97add1dd-7c49-4604-aa78-a077ee6923ce"
              },
              {
                "type": "iconbutton",
                "properties": {
                  "name": {
                    "icon": {
                      "name": "settings_rounded"
                    }
                  },
                  "bg": {
                    "color": {
                      "color": "surface"
                    }
                  },
                  "border": {
                    "border": {
                      "width": 2,
                      "color": "divider"
                    }
                  },
                  "radius": {
                    "radius": {
                      "topLeft": 0,
                      "topRight": 0,
                      "bottomLeft": 0,
                      "bottomRight": 0,
                      "token": "md"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  }
                },
                "editorId": "2bc21532-09c0-4969-8f61-b71715957f66"
              }
            ],
            "editorId": "a6156bef-3215-469e-8d2c-4a7880b5aee9"
          },
          {
            "type": "column",
            "properties": {
              "spacing": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "stack",
                "properties": {
                  "align": {
                    "align": {
                      "named": "center"
                    }
                  }
                },
                "children": [
                  {
                    "type": "container",
                    "properties": {
                      "width": {
                        "px": {
                          "value": 140,
                          "isInfinity": false
                        }
                      },
                      "height": {
                        "px": {
                          "value": 140,
                          "isInfinity": false
                        }
                      },
                      "bg": {
                        "color": {
                          "color": "secondary"
                        }
                      },
                      "radius": {
                        "radius": {
                          "topLeft": 0,
                          "topRight": 0,
                          "bottomLeft": 0,
                          "bottomRight": 0,
                          "token": "full"
                        }
                      },
                      "border": {
                        "border": {
                          "width": 3,
                          "color": "divider"
                        }
                      },
                      "shadow": {
                        "stringVal": {
                          "value": "lg"
                        }
                      },
                      "clip": {
                        "boolVal": {
                          "value": true
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "image",
                        "properties": {
                          "source_desc": {
                            "imageSource": {
                              "type": "IMAGE_SOURCE_TYPE_DESCRIPTION",
                              "value": "friendly professional chef portrait smiling"
                            }
                          },
                          "fit": {
                            "stringVal": {
                              "value": "cover"
                            }
                          }
                        },
                        "editorId": "2ad119c2-bd6c-4705-845e-8f7b7140dc9e"
                      }
                    ],
                    "editorId": "a785af77-7a88-4d55-a31e-dc2b512cf45b"
                  },
                  {
                    "type": "container",
                    "properties": {
                      "align": {
                        "align": {
                          "positional": {
                            "x": 1,
                            "y": 1
                          }
                        }
                      },
                      "width": {
                        "px": {
                          "value": 44,
                          "isInfinity": false
                        }
                      },
                      "height": {
                        "px": {
                          "value": 44,
                          "isInfinity": false
                        }
                      },
                      "bg": {
                        "color": {
                          "color": "accent"
                        }
                      },
                      "radius": {
                        "radius": {
                          "topLeft": 0,
                          "topRight": 0,
                          "bottomLeft": 0,
                          "bottomRight": 0,
                          "token": "full"
                        }
                      },
                      "border": {
                        "border": {
                          "width": 2,
                          "color": "divider"
                        }
                      },
                      "shadow": {
                        "stringVal": {
                          "value": "md"
                        }
                      },
                      "align_child": {
                        "align": {
                          "named": "center"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "icon",
                        "properties": {
                          "name": {
                            "icon": {
                              "name": "edit_rounded"
                            }
                          },
                          "size": {
                            "numberVal": {
                              "value": 20
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary_text"
                            }
                          }
                        },
                        "editorId": "2ea2df58-073f-4710-93c6-9a7c5f54b39f"
                      }
                    ],
                    "editorId": "200ed2bd-324a-4bee-8c74-4060d789a1b4"
                  }
                ],
                "editorId": "aa1f9e0e-561d-4688-a58b-fd4d11348d0e"
              },
              {
                "type": "column",
                "properties": {
                  "spacing": {
                    "stringVal": {
                      "value": "xs"
                    }
                  }
                },
                "children": [
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Chef Julian"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "headline_medium"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      },
                      "font_weight": {
                        "numberVal": {
                          "value": 900
                        }
                      }
                    },
                    "editorId": "240ecc27-93f3-4446-8a68-cdee8dd16020"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Pantry Master • Level 12"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "body_large"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "secondary_text"
                        }
                      }
                    },
                    "editorId": "00051593-6163-4b88-808f-0d15306e10aa"
                  }
                ],
                "editorId": "a433aeb6-9256-48a0-9dc9-f8c7027ebf57"
              }
            ],
            "editorId": "360b86b0-868b-4d95-838d-bbc9efa75c3b"
          },
          {
            "type": "row",
            "properties": {
              "spacing": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "@profile_stat",
                "properties": {
                  "value": {
                    "stringVal": {
                      "value": "42"
                    }
                  },
                  "label": {
                    "stringVal": {
                      "value": "Recipes Created"
                    }
                  }
                },
                "editorId": "b02637ed-e852-456a-9a53-5aa952f450f5"
              },
              {
                "type": "@profile_stat",
                "properties": {
                  "value": {
                    "stringVal": {
                      "value": "128"
                    }
                  },
                  "label": {
                    "stringVal": {
                      "value": "Meals Cooked"
                    }
                  }
                },
                "editorId": "30b6899a-c4dd-401e-8afc-e60a89d2185d"
              },
              {
                "type": "@profile_stat",
                "properties": {
                  "value": {
                    "stringVal": {
                      "value": "1.2k"
                    }
                  },
                  "label": {
                    "stringVal": {
                      "value": "XP Points"
                    }
                  }
                },
                "editorId": "d7183aef-1d05-4618-a277-53e002702a4c"
              }
            ],
            "editorId": "a617cf71-aa04-46c4-8f72-4614baa560f2"
          },
          {
            "type": "column",
            "properties": {
              "cross_align": {
                "align": {
                  "named": "start"
                }
              },
              "spacing": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "row",
                "properties": {
                  "spacing": {
                    "stringVal": {
                      "value": "sm"
                    }
                  }
                },
                "children": [
                  {
                    "type": "icon",
                    "properties": {
                      "name": {
                        "icon": {
                          "name": "favorite_rounded"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "error"
                        }
                      },
                      "size": {
                        "numberVal": {
                          "value": 24
                        }
                      }
                    },
                    "editorId": "bb28d845-54ac-40bc-802d-adfaf2c2203a"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Dietary Preferences"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "title_large"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      },
                      "font_weight": {
                        "numberVal": {
                          "value": 800
                        }
                      }
                    },
                    "editorId": "8e87282e-b145-441d-8a1b-0282f069e857"
                  }
                ],
                "editorId": "e2182fe4-b916-4b6f-b477-dedcff3ff46c"
              },
              {
                "type": "wrap",
                "properties": {
                  "spacing": {
                    "numberVal": {
                      "value": 0
                    }
                  }
                },
                "children": [
                  {
                    "type": "@preference_tag",
                    "properties": {
                      "label": {
                        "stringVal": {
                          "value": "Vegetarian"
                        }
                      },
                      "icon": {
                        "stringVal": {
                          "value": "eco_rounded"
                        }
                      },
                      "bg": {
                        "stringVal": {
                          "value": "success"
                        }
                      }
                    },
                    "editorId": "fabb7b39-d9c4-466c-8021-e96333aaeb1b"
                  },
                  {
                    "type": "@preference_tag",
                    "properties": {
                      "label": {
                        "stringVal": {
                          "value": "Gluten-Free"
                        }
                      },
                      "icon": {
                        "stringVal": {
                          "value": "grain_rounded"
                        }
                      },
                      "bg": {
                        "stringVal": {
                          "value": "secondary"
                        }
                      }
                    },
                    "editorId": "764bd3c9-2caf-4dc0-9386-ecf3f6ac0bcb"
                  },
                  {
                    "type": "@preference_tag",
                    "properties": {
                      "label": {
                        "stringVal": {
                          "value": "Dairy-Free"
                        }
                      },
                      "icon": {
                        "stringVal": {
                          "value": "water_drop_rounded"
                        }
                      },
                      "bg": {
                        "stringVal": {
                          "value": "accent"
                        }
                      }
                    },
                    "editorId": "3c7eab77-4ba8-4a3e-84a7-a7fc25baf4c0"
                  },
                  {
                    "type": "@preference_tag",
                    "properties": {
                      "label": {
                        "stringVal": {
                          "value": "Nut-Free"
                        }
                      },
                      "icon": {
                        "stringVal": {
                          "value": "block_rounded"
                        }
                      },
                      "bg": {
                        "color": {
                          "color": "#FFCDD2"
                        }
                      }
                    },
                    "editorId": "ac2daae5-5811-42bc-9528-2a823d9e0483"
                  },
                  {
                    "type": "@preference_tag",
                    "properties": {
                      "label": {
                        "stringVal": {
                          "value": "Low Carb"
                        }
                      },
                      "icon": {
                        "stringVal": {
                          "value": "speed_rounded"
                        }
                      },
                      "bg": {
                        "color": {
                          "color": "#E1F5FE"
                        }
                      }
                    },
                    "editorId": "935f6461-5eef-4bb6-88c4-a1848562e066"
                  }
                ],
                "editorId": "65571e8d-7c17-4554-a299-259ff9dc9bfc"
              }
            ],
            "editorId": "50d59191-1c25-418e-a7b2-141c2e5ca103"
          },
          {
            "type": "column",
            "properties": {
              "cross_align": {
                "align": {
                  "named": "start"
                }
              },
              "spacing": {
                "stringVal": {
                  "value": "md"
                }
              }
            },
            "children": [
              {
                "type": "row",
                "properties": {
                  "spacing": {
                    "stringVal": {
                      "value": "sm"
                    }
                  }
                },
                "children": [
                  {
                    "type": "icon",
                    "properties": {
                      "name": {
                        "icon": {
                          "name": "local_fire_department_rounded"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary"
                        }
                      },
                      "size": {
                        "numberVal": {
                          "value": 24
                        }
                      }
                    },
                    "editorId": "33e3dff2-3e37-4ab9-80fb-b4252968534a"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Cooking Skill Level"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "title_large"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      },
                      "font_weight": {
                        "numberVal": {
                          "value": 800
                        }
                      }
                    },
                    "editorId": "fcfdccc2-96d5-4a2c-b3e7-cc4d2d4698aa"
                  }
                ],
                "editorId": "6a73cb24-1545-4686-823a-b0ae0c489552"
              },
              {
                "type": "row",
                "properties": {
                  "spacing": {
                    "stringVal": {
                      "value": "md"
                    }
                  }
                },
                "children": [
                  {
                    "type": "@skill_card",
                    "properties": {
                      "icon": {
                        "stringVal": {
                          "value": "restaurant_rounded"
                        }
                      },
                      "title": {
                        "stringVal": {
                          "value": "Novice"
                        }
                      },
                      "desc": {
                        "stringVal": {
                          "value": "Still learning the basics of dicing."
                        }
                      },
                      "selected": {
                        "boolVal": {
                          "value": false
                        }
                      }
                    },
                    "editorId": "33f2ab5e-eb5e-40f3-a92c-d49f4dcf368f"
                  },
                  {
                    "type": "@skill_card",
                    "properties": {
                      "icon": {
                        "stringVal": {
                          "value": "skillet_rounded"
                        }
                      },
                      "title": {
                        "stringVal": {
                          "value": "Pro"
                        }
                      },
                      "desc": {
                        "stringVal": {
                          "value": "I can flip a pancake blindfolded."
                        }
                      },
                      "selected": {
                        "boolVal": {
                          "value": true
                        }
                      }
                    },
                    "editorId": "712421f0-13ad-4399-837e-32a1a7512486"
                  }
                ],
                "editorId": "bdf61eb7-bd23-4577-a010-a4da2e6812bb"
              }
            ],
            "editorId": "ae0dd5be-2b08-45c5-ab30-94e1fbc9a073"
          },
          {
            "type": "container",
            "properties": {
              "bg": {
                "color": {
                  "color": "surface"
                }
              },
              "radius": {
                "radius": {
                  "topLeft": 0,
                  "topRight": 0,
                  "bottomLeft": 0,
                  "bottomRight": 0,
                  "token": "xl"
                }
              },
              "padding": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "token": "lg"
                }
              },
              "border": {
                "border": {
                  "width": 2,
                  "color": "divider"
                }
              },
              "shadow": {
                "stringVal": {
                  "value": "sm"
                }
              }
            },
            "children": [
              {
                "type": "column",
                "properties": {
                  "cross_align": {
                    "align": {
                      "named": "start"
                    }
                  },
                  "spacing": {
                    "stringVal": {
                      "value": "md"
                    }
                  }
                },
                "children": [
                  {
                    "type": "row",
                    "properties": {
                      "align": {
                        "align": {
                          "named": "space_between"
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "column",
                        "properties": {
                          "cross_align": {
                            "align": {
                              "named": "start"
                            }
                          }
                        },
                        "children": [
                          {
                            "type": "text",
                            "properties": {
                              "content": {
                                "stringVal": {
                                  "value": "Weekly Nutrition"
                                }
                              },
                              "style": {
                                "textStyle": {
                                  "styleName": "title_medium"
                                }
                              },
                              "color": {
                                "color": {
                                  "color": "primary_text"
                                }
                              },
                              "font_weight": {
                                "numberVal": {
                                  "value": 700
                                }
                              }
                            },
                            "editorId": "30e9f5a8-d90c-4514-b6be-34d39563b12e"
                          },
                          {
                            "type": "text",
                            "properties": {
                              "content": {
                                "stringVal": {
                                  "value": "Protein focus this week"
                                }
                              },
                              "style": {
                                "textStyle": {
                                  "styleName": "body_small"
                                }
                              },
                              "color": {
                                "color": {
                                  "color": "secondary_text"
                                }
                              }
                            },
                            "editorId": "48a91677-b8d8-4ba1-a162-c44a47199c93"
                          }
                        ],
                        "editorId": "fe3af34f-6497-437f-8a10-c593314a1a92"
                      },
                      {
                        "type": "icon",
                        "properties": {
                          "name": {
                            "icon": {
                              "name": "insights_rounded"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary"
                            }
                          }
                        },
                        "editorId": "47c892ac-c693-4cf5-a5e0-01403db078ef"
                      }
                    ],
                    "editorId": "d9df0c3e-5b15-4fce-b562-f0a535d503d1"
                  },
                  {
                    "type": "container",
                    "properties": {
                      "height": {
                        "px": {
                          "value": 180,
                          "isInfinity": false
                        }
                      },
                      "width": {
                        "px": {
                          "value": "Infinity",
                          "isInfinity": true
                        }
                      }
                    },
                    "children": [
                      {
                        "type": "bar_chart",
                        "properties": {
                          "data": {
                            "stringVal": {
                              "value": "65,80,45,90,70,55,85"
                            }
                          },
                          "labels": {
                            "stringVal": {
                              "value": "M,T,W,T,F,S,S"
                            }
                          },
                          "color": {
                            "color": {
                              "color": "primary"
                            }
                          },
                          "bar_width": {
                            "numberVal": {
                              "value": 24
                            }
                          },
                          "bar_radius": {
                            "numberVal": {
                              "value": 8
                            }
                          },
                          "show_labels": {
                            "boolVal": {
                              "value": true
                            }
                          }
                        },
                        "editorId": "426bf168-7cb4-466b-b5e4-ac986a69c4e4"
                      }
                    ],
                    "editorId": "ebcbd781-db8c-42a0-b16f-b46fab32a5d8"
                  }
                ],
                "editorId": "ab533540-fa45-4e40-9aca-403e00cf47f4"
              }
            ],
            "editorId": "698c9bac-d743-49ba-8f43-4aac4d82a2cf"
          },
          {
            "type": "column",
            "properties": {
              "cross_align": {
                "align": {
                  "named": "start"
                }
              },
              "spacing": {
                "stringVal": {
                  "value": "sm"
                }
              }
            },
            "children": [
              {
                "type": "text",
                "properties": {
                  "content": {
                    "stringVal": {
                      "value": "About Me"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "title_medium"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  },
                  "font_weight": {
                    "numberVal": {
                      "value": 700
                    }
                  }
                },
                "editorId": "0b9933cc-b121-4dbf-98b6-ed84213ae9b1"
              },
              {
                "type": "container",
                "properties": {
                  "bg": {
                    "color": {
                      "color": "surface"
                    }
                  },
                  "radius": {
                    "radius": {
                      "topLeft": 0,
                      "topRight": 0,
                      "bottomLeft": 0,
                      "bottomRight": 0,
                      "token": "lg"
                    }
                  },
                  "padding": {
                    "edgeInsets": {
                      "top": 0,
                      "right": 0,
                      "bottom": 0,
                      "left": 0,
                      "token": "md"
                    }
                  },
                  "border": {
                    "border": {
                      "width": 2,
                      "color": "divider"
                    }
                  },
                  "width": {
                    "px": {
                      "value": "Infinity",
                      "isInfinity": true
                    }
                  }
                },
                "children": [
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Passionate about turning simple ingredients into extraordinary meals. I love Mediterranean flavors and quick 20-minute dinners!"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "body_medium"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      }
                    },
                    "editorId": "fd689cb3-bae4-4752-8fd0-370deff28fe0"
                  }
                ],
                "editorId": "8cc460b2-8e99-4257-9b02-15f19e2b1c74"
              }
            ],
            "editorId": "9952eaaa-8dcf-4118-8dd7-0a5c52411a03"
          },
          {
            "type": "container",
            "properties": {
              "bg": {
                "color": {
                  "color": "primary"
                }
              },
              "radius": {
                "radius": {
                  "topLeft": 0,
                  "topRight": 0,
                  "bottomLeft": 0,
                  "bottomRight": 0,
                  "token": "xl"
                }
              },
              "padding": {
                "edgeInsets": {
                  "top": 0,
                  "right": 0,
                  "bottom": 0,
                  "left": 0,
                  "token": "lg"
                }
              },
              "border": {
                "border": {
                  "width": 2,
                  "color": "divider"
                }
              },
              "shadow": {
                "stringVal": {
                  "value": "lg"
                }
              },
              "align_child": {
                "align": {
                  "named": "center"
                }
              }
            },
            "children": [
              {
                "type": "row",
                "properties": {
                  "main_size": {
                    "stringVal": {
                      "value": "min"
                    }
                  },
                  "spacing": {
                    "stringVal": {
                      "value": "md"
                    }
                  }
                },
                "children": [
                  {
                    "type": "icon",
                    "properties": {
                      "name": {
                        "icon": {
                          "name": "check_circle_rounded"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "on_primary"
                        }
                      },
                      "size": {
                        "numberVal": {
                          "value": 24
                        }
                      }
                    },
                    "editorId": "d7caae11-6bea-451b-8913-658ac41aeb50"
                  },
                  {
                    "type": "text",
                    "properties": {
                      "content": {
                        "stringVal": {
                          "value": "Save Profile Changes"
                        }
                      },
                      "style": {
                        "textStyle": {
                          "styleName": "title_medium"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "on_primary"
                        }
                      },
                      "font_weight": {
                        "numberVal": {
                          "value": 700
                        }
                      }
                    },
                    "editorId": "853d5cf9-9bf8-41c6-8d19-20cd5379e7a6"
                  }
                ],
                "editorId": "d65aed12-7da4-4f6f-bef6-60dc1d5add1d"
              }
            ],
            "editorId": "b903dd0f-6fc3-430c-80f5-cf9ed686c74c"
          },
          {
            "type": "sizedbox",
            "properties": {
              "height": {
                "stringVal": {
                  "value": "xl"
                }
              }
            },
            "editorId": "12e6e084-b8e8-4151-b435-d788dbad0f8e"
          }
        ],
        "editorId": "e3a75a7d-08d3-4fe3-8e9b-9fdfecf7143a"
      }
    ],
    "editorId": "b6eb4d3e-31c0-4493-9d0d-7066b9ad52f6"
  },
  "components": [
    {
      "name": "profile_stat",
      "root": {
        "type": "container",
        "properties": {
          "bg": {
            "color": {
              "color": "surface"
            }
          },
          "radius": {
            "radius": {
              "topLeft": 0,
              "topRight": 0,
              "bottomLeft": 0,
              "bottomRight": 0,
              "token": "lg"
            }
          },
          "padding": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "token": "md"
            }
          },
          "border": {
            "border": {
              "width": 2,
              "color": "divider"
            }
          },
          "shadow": {
            "stringVal": {
              "value": "sm"
            }
          },
          "expanded": {
            "expanded": {
              "enabled": true,
              "flex": 1
            }
          }
        },
        "children": [
          {
            "type": "column",
            "properties": {
              "spacing": {
                "stringVal": {
                  "value": "xs"
                }
              }
            },
            "children": [
              {
                "type": "text",
                "properties": {
                  "content": {
                    "slot": {
                      "name": "value"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "title_large"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  },
                  "font_weight": {
                    "numberVal": {
                      "value": 800
                    }
                  }
                },
                "editorId": "87a78cbb-6f0a-455d-90ef-40a03e9c5f48"
              },
              {
                "type": "text",
                "properties": {
                  "content": {
                    "slot": {
                      "name": "label"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "label_small"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "secondary_text"
                    }
                  }
                },
                "editorId": "7d0fbd90-349b-46bc-8c8e-e6bf77c96f16"
              }
            ],
            "editorId": "3e8f01f5-2960-40d6-9676-30ff0ec81b15"
          }
        ],
        "editorId": "8ef78409-2614-4935-aecf-b58380f59dee"
      }
    },
    {
      "name": "preference_tag",
      "root": {
        "type": "container",
        "properties": {
          "bg": {
            "slot": {
              "name": "bg"
            }
          },
          "radius": {
            "radius": {
              "topLeft": 0,
              "topRight": 0,
              "bottomLeft": 0,
              "bottomRight": 0,
              "token": "full"
            }
          },
          "padding": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "topToken": "md",
              "rightToken": "sm",
              "bottomToken": "md",
              "leftToken": "sm"
            }
          },
          "border": {
            "border": {
              "width": 2,
              "color": "divider"
            }
          },
          "margin": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "rightToken": "sm",
              "bottomToken": "sm"
            }
          }
        },
        "children": [
          {
            "type": "row",
            "properties": {
              "spacing": {
                "stringVal": {
                  "value": "sm"
                }
              },
              "main_size": {
                "stringVal": {
                  "value": "min"
                }
              }
            },
            "children": [
              {
                "type": "icon",
                "properties": {
                  "name": {
                    "slot": {
                      "name": "icon"
                    }
                  },
                  "size": {
                    "numberVal": {
                      "value": 16
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  }
                },
                "editorId": "6a526f16-d83e-4196-806c-7be961955081"
              },
              {
                "type": "text",
                "properties": {
                  "content": {
                    "slot": {
                      "name": "label"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "body_medium"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  },
                  "font_weight": {
                    "numberVal": {
                      "value": 600
                    }
                  }
                },
                "editorId": "4f85729b-ff4e-4541-bc3f-cd08ba79fd3c"
              }
            ],
            "editorId": "7e12f527-7593-48ef-a699-27da97d4c780"
          }
        ],
        "editorId": "9eb0bfef-69d0-4f5a-9447-a3cbaa4e35e9"
      }
    },
    {
      "name": "skill_card",
      "root": {
        "type": "container",
        "properties": {
          "bg": {
            "conditional": {
              "conditionSlot": "selected",
              "trueValue": {
                "color": {
                  "color": "accent"
                }
              },
              "falseValue": {
                "color": {
                  "color": "surface"
                }
              }
            }
          },
          "radius": {
            "radius": {
              "topLeft": 0,
              "topRight": 0,
              "bottomLeft": 0,
              "bottomRight": 0,
              "token": "xl"
            }
          },
          "padding": {
            "edgeInsets": {
              "top": 0,
              "right": 0,
              "bottom": 0,
              "left": 0,
              "token": "lg"
            }
          },
          "border": {
            "border": {
              "width": 2,
              "color": "divider"
            }
          },
          "shadow": {
            "conditional": {
              "conditionSlot": "selected",
              "trueValue": {
                "stringVal": {
                  "value": "md"
                }
              },
              "falseValue": {
                "stringVal": {
                  "value": "sm"
                }
              }
            }
          },
          "expanded": {
            "expanded": {
              "enabled": true,
              "flex": 1
            }
          }
        },
        "children": [
          {
            "type": "column",
            "properties": {
              "spacing": {
                "stringVal": {
                  "value": "sm"
                }
              }
            },
            "children": [
              {
                "type": "container",
                "properties": {
                  "width": {
                    "px": {
                      "value": 48,
                      "isInfinity": false
                    }
                  },
                  "height": {
                    "px": {
                      "value": 48,
                      "isInfinity": false
                    }
                  },
                  "bg": {
                    "color": {
                      "color": "background"
                    }
                  },
                  "radius": {
                    "radius": {
                      "topLeft": 0,
                      "topRight": 0,
                      "bottomLeft": 0,
                      "bottomRight": 0,
                      "token": "lg"
                    }
                  },
                  "border": {
                    "border": {
                      "width": 2,
                      "color": "divider"
                    }
                  },
                  "align_child": {
                    "align": {
                      "named": "center"
                    }
                  }
                },
                "children": [
                  {
                    "type": "icon",
                    "properties": {
                      "name": {
                        "slot": {
                          "name": "icon"
                        }
                      },
                      "color": {
                        "color": {
                          "color": "primary_text"
                        }
                      },
                      "size": {
                        "numberVal": {
                          "value": 24
                        }
                      }
                    },
                    "editorId": "09251d94-656d-4809-b73c-c17f29334ee8"
                  }
                ],
                "editorId": "fe31e93d-5460-4a5e-9e2d-99bd5e188eed"
              },
              {
                "type": "text",
                "properties": {
                  "content": {
                    "slot": {
                      "name": "title"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "title_medium"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "primary_text"
                    }
                  },
                  "font_weight": {
                    "numberVal": {
                      "value": 700
                    }
                  }
                },
                "editorId": "04dd5cc3-c0c4-4ff0-95bb-2e89e40f2a23"
              },
              {
                "type": "text",
                "properties": {
                  "content": {
                    "slot": {
                      "name": "desc"
                    }
                  },
                  "style": {
                    "textStyle": {
                      "styleName": "body_small"
                    }
                  },
                  "color": {
                    "color": {
                      "color": "secondary_text"
                    }
                  },
                  "max_lines": {
                    "numberVal": {
                      "value": 2
                    }
                  },
                  "overflow": {
                    "stringVal": {
                      "value": "ellipsis"
                    }
                  }
                },
                "editorId": "38b1b06b-d335-4ad1-824f-aa9aa69928e6"
              }
            ],
            "editorId": "fdff6ec2-f9d2-469a-8227-a49fccf3c1d7"
          }
        ],
        "editorId": "cd598b54-fe25-4a2e-ad9e-c0c03a455da3"
      }
    }
  ]
}
```