---
title: The Subscription Object
has_children: false
parent: Recharge Honest Paws
grand-parent: Data Schema
nav_order: 1
---
# The subscription object
{: .no_toc }

Subscriptions are individual items a customer receives on a recurring basis.

A subscription is a product added to an address. A Customer can create only 1 subscription of the same product on 1 address. A Customer can create multiple subscriptions of the same product but only if Customer has chosen different address object.

If store owner wants to sell multiple products as one subscription on 1 address it can be done by creating a product in Shopify that consists of multiple products e.g. 3 types of vegetables in the box, set of different shirts, etc. This multiple products appear on the store as 1 product, therefore it can be sold in a single subscription to 1 or more addresses.

## Attributes
|Field name |Data type |Description |
|:----------|:---------|:-----------| 
|id|integer|Unique numeric identifier for the subscription.|
|address_id|integer|Unique numeric identifier for the address the subscription is associated with.|
|cancellation_reason|string|Reason provided for cancellation.|
|cancellation_reason_comment|string|Additional comment for cancellation.|
|cancelled_at|string|The time the subscription was cancelled.|
|charge_interval_frequency|string|The number of units (specified in order_interval_unit) between each charge. For example, order_interval_unit=month and charge_interval_frequency=3, indicate charge every 3 months. Charges must use the same unit types as orders. Max value: 1000|
|created_at|integer|The time the subscription was created.|
|commit_update|boolean|Specifies whether the regeneration of the connected charge should happen right away, or after a 5 second delay (when value is set to False).|
|customer_id|integer|Unique numeric identifier for the customer the subscription is tied to.|
|email|string|The email address of the customer.|
|expire_after_specific_number_of_charges|integer|Set the number of charges until subscription expires.|
|has_queued_charges|boolean|Retrieves 1 if there is queued charge. Otherwise, retrieves 0.|
|is_prepaid|boolean|Value is set to True if it is a prepaid item.|
|is_skippable|boolean|Value is set to True if it is not a prepaid item|
|is_swappable|boolean|Value is set to True if it is not a prepaid item and if in Customer portal settings swap is allowed for customers.|
|max_retries_reached|boolean|Retrieves 1 if charge has an error max retries reached. Otherwise, retrieves 0.|
|next_charge_scheduled_at|string|Date of the next charge for the subscription.|
|order_day_of_month|integer|The set day of the month order is created. Default is that there isn’t a strict day of the month when the order is created. This is only applicable to subscriptions with order_interval_unit = “month”.|
|order_day_of_week|integer|The set day of the week order is created. Default is that there isn’t a strict day of the week order is created. This is only applicable to subscriptions with order_interval_unit = “week”. Value of 0 equals to Monday, 1 to Tuesday etc.|
|order_interval_frequency|string|The number of units (specified in order_interval_unit) between each order. For example, order_interval_unit=month and order_interval_frequency=3, indicate order every 3 months. Max value: 1000|
|order_interval_unit|string|The frequency which a subscription should have the order created with. Valid values are “day”,“week”, and “month”.|
|price|float|The price of the item before discounts, taxes, or shipping have been applied.|
|product_title|string|The name of the product in a shop’s catalog.|
|properties|array|of dictionary objects|
|A|list|of line item objects, each one containing information about the subscription. Custom key-value pairs can be installed here, they will appear on the connected queued charge and after it is processed on the order itself.|
|quantity|integer|The number of items in the subscription.|
|recharge_product_id|integer|Unique number identifier of the product in ReCharge.|
|shopify_product_id|integer|Unique number identifier of the product in Shopify.|
|shopify_variant_id|integer|Unique number identifier of the product variant in Shopify.|
|sku|string|A unique identifier of the item in the fulfillment. In cases where SKU is blank, it will be dynamically pulled whenever it is used.|
|sku_override|boolean|Flag that is automatically updated to true when SKU is passed on create or update. When sku_override is true, the sku on the subscription will be used to generate charges and orders. When sku_override is false, Recharge will dynamically fetch the SKU from the corresponding shopify variant.|
|status|string|The status of the subscription. Valid values:
• ACTIVE - The subscription is active.
• CANCELLED - The subscription has been cancelled.
• EXPIRED - The subscription has expired. This occurs when the maximum number of charges for a product has been reached.
|variant_title|string|The name of the variant in a shop’s catalog.|

---

#### Table of contents
{: .no_toc }

1. Table of contents
{:toc}

---



---
```
This page is updated on Jan 11th, 2021.
```
