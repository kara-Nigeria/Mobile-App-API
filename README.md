# Mobile-App-API
API documentation for the Mobile App Devs to interact with.

**API Documentation: Retrieve Mega Deals from the main Website**

**Description:**
This API endpoint allows you to retrieve all the deals categorized under "Mega Deals" from our main Magento website (Kara.com.ng). The deals are sorted by their creation date.

**Endpoint:**
```
  GET https://kara.com.ng/rest/all/V1/products
```

**Mandatory Parameters:**
- `searchCriteria[sortOrders][0][field]`: Specifies the field to sort the results. In this case, it's set to `created_at` to sort by creation date.
- `searchCriteria[filterGroups][0][filters][0][field]`: Specifies the field to filter the results. It's set to `category_id` to filter by category ID.
- `searchCriteria[filterGroups][0][filters][0][value]`: Specifies the value to filter by. In this case, it's set to `580`, which corresponds to the category ID of "Mega Deals".

**Response:**
The API returns a JSON response containing details of all the products categorized under "Mega Deals". Each product object includes information such as its ID, name, price, description, and other relevant attributes.

**Example Request:**
```
  GET https://kara.com.ng/rest/all/V1/products?searchCriteria[sortOrders][0][field]=created_at&searchCriteria[filterGroups][0][filters][0][field]=category_id&searchCriteria[filterGroups][0][filters][0][value]=580
```

**Example Response:**
```json
{
    "items": [
        {
            "id": 10470,
            "sku": "HP623KAOS",
            "name": "HP 26A Cartridge (Compatible)",
            "attribute_set_id": 73,
            "price": 35000,
            "status": 1,
            "visibility": 4,
            "type_id": "simple",
            "created_at": "2024-03-08 13:55:52",
            "updated_at": "2024-03-08 14:25:11",
            "extension_attributes": {
                "website_ids": [
                    1
                ],
                "category_links": [
                    {
                        "position": 0,
                        "category_id": "63"
                    },
                    {
                        "position": 0,
                        "category_id": "90"
                    },
                    {
                        "position": 0,
                        "category_id": "267"
                    },
                    {
                        "position": 0,
                        "category_id": "580"
                    }
                ]
            },
            "product_links": [],
            "options": [],
            "media_gallery_entries": [
                {
                    "id": 22265,
                    "media_type": "image",
                    "label": null,
                    "position": 1,
                    "disabled": false,
                    "types": [
                        "image",
                        "small_image",
                        "thumbnail",
                        "swatch_image",
                        "weltpixel_hover_image"
                    ],
                    "file": "/l/d/ld_hp_cf226acta_compat_bk.jpg"
                }
            ],
            "tier_prices": [],
            "custom_attributes": [
                {
                    "attribute_code": "image",
                    "value": "/l/d/ld_hp_cf226acta_compat_bk.jpg"
                },
                {
                    "attribute_code": "url_key",
                    "value": "hp-26a-cartridge-compatible"
                },
                {
                    "attribute_code": "gift_message_available",
                    "value": "2"
                },
                {
                    "attribute_code": "wesupply_estimation_display",
                    "value": "1"
                },
                {
                    "attribute_code": "weltpixel_exclude_from_sitemap",
                    "value": "0"
                },
                {
                    "attribute_code": "finger_print_reader",
                    "value": "0"
                },
                {
                    "attribute_code": "small_image",
                    "value": "/l/d/ld_hp_cf226acta_compat_bk.jpg"
                },
                {
                    "attribute_code": "meta_title",
                    "value": "Enhance Your Printing Experience with HP 26A Compatible Cartridge – Available at KARA Nigeria"
                },
                {
                    "attribute_code": "options_container",
                    "value": "container2"
                },
                {
                    "attribute_code": "brand",
                    "value": "272"
                },
                {
                    "attribute_code": "thumbnail",
                    "value": "/l/d/ld_hp_cf226acta_compat_bk.jpg"
                },
                {
                    "attribute_code": "meta_keyword",
                    "value": "HP 26A Compatible Cartridge, Printing Supplies, Printer Cartridges, Office Printing Solutions, Affordable Printing Options, Quality Print Products, Sustainable Printing Practices, Eco-Friendly Cartridges"
                },
                {
                    "attribute_code": "swatch_image",
                    "value": "/l/d/ld_hp_cf226acta_compat_bk.jpg"
                },
                {
                    "attribute_code": "meta_description",
                    "value": "Experience unmatched print quality with the HP 26A Compatible Cartridge, available at KARA Nigeria. Rigorously tested for consistency and precision, this cartridge rivals OEM standards, maintaining the integrity ETC"
                },
                {
                    "attribute_code": "weltpixel_hover_image",
                    "value": "/l/d/ld_hp_cf226acta_compat_bk.jpg"
                },
                {
                    "attribute_code": "msrp_display_actual_price_type",
                    "value": "0"
                },
                {
                    "attribute_code": "tax_class_id",
                    "value": "2"
                },
                {
                    "attribute_code": "title_rewrite",
                    "value": "HP 26A Cartridge (Compatible)"
                },
                {
                    "attribute_code": "required_options",
                    "value": "0"
                },
                {
                    "attribute_code": "has_options",
                    "value": "0"
                },
                {
                    "attribute_code": "category_ids",
                    "value": [
                        "63",
                        "90",
                        "267",
                        "580"
                    ]
                },
                {
                    "attribute_code": "is_featured",
                    "value": "1"
                },
                {
                    "attribute_code": "description",
                    "value": "<h1><strong><span style=\"font-size: 16px;\">HP 26A CARTRIDGE ( COMPATIBLE) | BEST PRICE @ KARA NIGERIA</span></strong></h1>\r\n<h1><strong><span style=\"font-size: 16px;\">PRODUCT OVERVIEW: </span></strong></h1>\r\n<p><span style=\"font-size: 16px;\">The HP 26A cartridge is a compatible toner cartridge that is used in a variety of HP LaserJet Pro printers. It is a black toner cartridge that can print up to 3,100 pages. Compatible cartridges are typically made by third-party manufacturers and are not manufactured by HP. They are typically less expensive than OEM (Original Equipment Manufacturer) cartridges, but they may not be of the same quality.</span></p>\r\n<p><span style=\"font-size: 16px;\">When it comes to optimizing printing performance while managing costs effectively, the HP 26A Compatible Cartridge emerges as a standout choice. Available at KARA Nigeria, this cartridge delivers exceptional quality, reliability, and affordability. </span></p>\r\n<p><span style=\"font-size: 16px;\">At KARA Nigeria, the HP 26A Compatible Cartridge offers significant cost savings without compromising on performance. Its competitive pricing structure ensures that businesses and individuals alike can enjoy premium printing quality at a fraction of the cost of OEM cartridges. Say goodbye to budget constraints and hello to affordability with the HP 26A Compatible Cartridge from KARA Nigeria.</span></p>\r\n<p><span style=\"font-size: 16px;\">By choosing the HP 26A Compatible Cartridge from KARA Nigeria, you're making an eco-friendly decision. Crafted from sustainable materials and manufactured using environmentally conscious practices, this cartridge helps reduce electronic waste and conserves valuable resources. Join the movement towards sustainability while enjoying exceptional print quality with the HP 26A Compatible Cartridge.</span></p>\r\n<h2><strong><span style=\"font-size: 16px;\">SPECIFICATION: </span></strong></h2>\r\n<ul>\r\n<li><span style=\"font-family: verdana, geneva; font-size: 16px;\">Color(s) of print cartridges: Black</span></li>\r\n<li><span style=\"font-family: verdana, geneva; font-size: 16px;\">Print technology: Laser</span></li>\r\n<li><span style=\"font-family: verdana, geneva; font-size: 16px;\">Page yield (black and white): 3,100 pages</span></li>\r\n</ul>\r\n<p> </p>"
                }
            ]
        },
        {
            "id": 10468,
            "sku": "FBC2001KAOS",
            "name": "Famicare 30A Battery Charger",
            "attribute_set_id": 73,
            "price": 80500,
            "status": 1,
            "visibility": 4,
            "type_id": "simple",
            "created_at": "2024-03-07 16:40:54",
            "updated_at": "2024-03-08 11:40:05",
            "extension_attributes": {
                "website_ids": [
                    1
                ],
                "category_links": [
                    {
                        "position": 0,
                        "category_id": "580"
                    },
                    {
                        "position": 0,
                        "category_id": "304"
                    },
                    {
                        "position": 0,
                        "category_id": "311"
                    },
                    {
                        "position": 0,
                        "category_id": "333"
                    }
                ]
            },
            "product_links": [],
            "options": [],
            "media_gallery_entries": [
                {
                    "id": 22262,
                    "media_type": "image",
                    "label": null,
                    "position": 1,
                    "disabled": false,
                    "types": [
                        "image",
                        "small_image",
                        "thumbnail",
                        "swatch_image",
                        "weltpixel_hover_image"
                    ],
                    "file": "/f/a/famicare_30a_battery_charger.jpg"
                },
                {
                    "id": 22263,
                    "media_type": "image",
                    "label": null,
                    "position": 2,
                    "disabled": false,
                    "types": [],
                    "file": "/f/a/famicare_30a_back.jpg"
                }
            ],
            "tier_prices": [],
            "custom_attributes": [
                {
                    "attribute_code": "image",
                    "value": "/f/a/famicare_30a_battery_charger.jpg"
                },
                {
                    "attribute_code": "url_key",
                    "value": "famicare-30a-battery-charger"
                },
                {
                    "attribute_code": "gift_message_available",
                    "value": "2"
                },
                {
                    "attribute_code": "wesupply_estimation_display",
                    "value": "1"
                },
                {
                    "attribute_code": "weltpixel_exclude_from_sitemap",
                    "value": "0"
                },
                {
                    "attribute_code": "finger_print_reader",
                    "value": "0"
                },
                {
                    "attribute_code": "small_image",
                    "value": "/f/a/famicare_30a_battery_charger.jpg"
                },
                {
                    "attribute_code": "meta_title",
                    "value": "Famicare 30A Battery Charger"
                },
                {
                    "attribute_code": "options_container",
                    "value": "container2"
                },
                {
                    "attribute_code": "brand",
                    "value": "324"
                },
                {
                    "attribute_code": "thumbnail",
                    "value": "/f/a/famicare_30a_battery_charger.jpg"
                },
                {
                    "attribute_code": "meta_keyword",
                    "value": "Famicare 30A Battery Charger"
                },
                {
                    "attribute_code": "swatch_image",
                    "value": "/f/a/famicare_30a_battery_charger.jpg"
                },
                {
                    "attribute_code": "meta_description",
                    "value": "Famicare 30A Battery Charger "
                },
                {
                    "attribute_code": "weltpixel_hover_image",
                    "value": "/f/a/famicare_30a_battery_charger.jpg"
                },
                {
                    "attribute_code": "msrp_display_actual_price_type",
                    "value": "0"
                },
                {
                    "attribute_code": "tax_class_id",
                    "value": "2"
                },
                {
                    "attribute_code": "required_options",
                    "value": "0"
                },
                {
                    "attribute_code": "has_options",
                    "value": "0"
                },
                {
                    "attribute_code": "category_ids",
                    "value": [
                        "580",
                        "304",
                        "311",
                        "333"
                    ]
                },
                {
                    "attribute_code": "is_featured",
                    "value": "1"
                },
                {
                    "attribute_code": "country_of_manufacture",
                    "value": "CN"
                },
                {
                    "attribute_code": "description",
                    "value": "<p><strong><span style=\"font-size: 16px;\">FAMICARE 30A BATTERY CHARGER | BEST PLACE TO SHOP FOR LESS....</span></strong></p>\r\n<h1><strong><span style=\"font-size: 16px;\">PRODUCT DESCRIPTION: </span></strong></h1>\r\n<h2><span style=\"font-size: 16px;\">The Famicare 30A Battery Charger is a heavy-duty charger that can be used for 12V or 24V batteries. It is a popular choice for charging car batteries, deep cycle batteries, and other types of rechargeable batteries.Famicare 30AH is highly efficient smart battery charger suitable to support your inverters for big battery banks charging. It efficient for home and offices usage. It can charge your Deep cycle inverter battery with PHCN electricity or Generator in the shortest possible time depending on the number of batteries you are using, and it is also capable of supplying a prolonged back-up to your inverter to make it faster in charging of your batteries.Like 100AH ,200AH,150AH battery.</span></h2>\r\n<h2><strong><span style=\"font-size: 16px;\">FEATURES:</span></strong></h2>\r\n<ul>\r\n<li> With efficient in-built charger </li>\r\n<li> Over load protection</li>\r\n<li> Over voltage protection </li>\r\n<li> Temperature protection</li>\r\n<li>  Reverse polarity protection </li>\r\n<li> DC under voltage protection </li>\r\n<li> Output short circuit protection </li>\r\n<li> Input high and low voltage protection </li>\r\n<li> Lack-voltage alarm </li>\r\n<li> Lack-voltage protection </li>\r\n<li> AC input low-voltage protection</li>\r\n<li> AC input over -voltage protection</li>\r\n</ul>\r\n<p> </p>\r\n<p> </p>\r\n<div class=\"list -features\"> </div>\r\n<p> </p>"
                }
            ]
        }
      ],
    "search_criteria": {
        "filter_groups": [
            {
                "filters": [
                    {
                        "field": "category_id",
                        "value": "580",
                        "condition_type": "eq"
                    }
                ]
            }
        ],
        "sort_orders": [
            {
                "field": "created_at",
                "direction": null
            }
        ],
        "page_size": 3
    },
    "total_count": 12
}
```
