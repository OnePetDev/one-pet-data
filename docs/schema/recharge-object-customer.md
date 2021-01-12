---
title: The Customer Object
has_children: false
parent: Recharge Honest Paws
grand_parent: Data Schema
nav_order: 2
---
# The customer object
{: .no_toc }

The Customer object holds account and billing information. Email is unique on the customer; no two customers for a store can have the same email. Address is the child of the customer object. There can be many child addresses on a customer, but only one parent customer per address.

## Attributes

|Field name |Data type |Description |
|:----------|:---------|:-----------|
|id|integer|Unique numeric identifier for the customer.|
|billing_address1|string|The customer’s billing address.|
|billing_address2|string|An additional field for the customer’s billing address.|
|billing_city|string|The customer’s billing city.|
|billing_company|string|The customer’s billing company.|
|billing_country|string|The customer’s billing country.|
|billing_first_name|string|The customer’s billing first name. Required when creating a customer.|
|billing_last_name|string|The customer’s billing last name. Required when creating a customer.|
|billing_phone|string|The customer’s billing phone number.|
|billing_province|string|The customer’s billing province or state name.|
|billing_zip|string|The customer’s billing zip or postal code.|
|created_at|datetime|The date and time when the customer was created.|
|email|string|The email address of the customer.|
|first_charge_processed_at|datetime|Date when first charge was processed for the customer.|
|first_name|string|The customer’s first name.|
|has_card_error_in_dunning|boolean|Does have a credit card in dunning, can be true and false.|
|has_valid_payment_method|boolean|Is the payment method valid or not, can be true and false.|
|hash|string|The unique string identifier used in a customers portal link.|
|last_name|string|The customer’s last name.|
|number_active_subscriptions|integer|The number of active subscriptions for the customer.|
|number_subscriptions|integer|The number of subscriptions for the customer.|
|processor_type|string|What the merchant processor customer is stored on.|
|reason_payment_method_not_valid|string|Why payment method is not valid.|
|shopify_customer_id|string|Shopify’s unique identifier for the customer.|
|status|string|Customer’s status, can be ACTIVE and INACTIVE.|
|updated_at|datetime|The date and time when the customer was last updated.|

---
```
This page is updated on Jan 11th, 2021.
```
