Dataset description

This dataset contains in Parquet format all price information contained in the Open Prices database. The dataset is updated daily.

Here is a description of the most important columns:

id: The ID of the price in DB
product_code: The barcode of the product, null if the product is a "raw" product (fruit, vegetable, etc.)
category_tag: The category of the product, only present for "raw" products. We follow Open Food Facts category taxonomy for category IDs.
labels_tags: The labels of the product, only present for "raw" products. We follow Open Food Facts label taxonomy for label IDs.
origins_tags: The origins of the product, only present for "raw" products. We follow Open Food Facts origin taxonomy for origin IDs.
price: The price of the product, with the discount if any.
price_is_discounted: Whether the price is discounted or not.
price_without_discount: The price of the product without discount, null if the price is not discounted.
price_per: The unit for which the price is given (e.g. "KILOGRAM", "UNIT")
currency: The currency of the price
location_osm_id: The OpenStreetMap ID of the location where the price was recorded. We use OpenStreetMap to identify uniquely the store where the price was recorded.
location_osm_type: The type of the OpenStreetMap location (e.g. "NODE", "WAY")
location_id: The ID of the location in the Open Prices database
date: The date when the price was recorded
proof_id: The ID of the proof of the price in the Open Prices DB
owner: a hash of the owner of the price, for privacy.
created: The date when the price was created in the Open Prices DB
updated: The date when the price was last updated in the Open Prices DB
proof_file_path: The path to the proof file in the Open Prices DB
proof_type: The type of the proof. Possible values are RECEIPT, PRICE_TAG, GDPR_REQUEST, SHOP_IMPORT
proof_date: The date of the proof
proof_currency: The currency of the proof, should be the same as the price currency
proof_created: The datetime when the proof was created in the Open Prices DB
proof_updated: The datetime when the proof was last updated in the Open Prices DB
location_osm_display_name: The display name of the OpenStreetMap location
location_osm_address_city: The city of the OpenStreetMap location
location_osm_address_postcode: The postcode of the OpenStreetMap location

