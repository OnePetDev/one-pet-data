---
title: Honest Paws Klaviyo lists
nav_order: 2
---
# Klaviyo lists

The following Klaviyo lists are sent from the One Pet Data Lake.

## List of Active Subscribers

Name of list in Klaviyo: **onepetdata_Active Subscribers**

Klaviyo list ID: [ ]( )

### Definition

Customers with at least one active subscription. Updated every 2 hours.

### Attributes

**onepetdata_subs_start_dates**

The dates when subscriptions were started. In case of multiple subscriptions, comma separated list of dates.

```
Bug: Klaviyo user interface shows one date even when multiple dates are present.
```

**onepetdata_subs_product_name**

Complete name of the Subscription product as written on the Shopify product page.

**onepetdata_subs_variant_name**

Product variant name as written on Shopify. Empty when no variants are defined.

**onepetdata_subs_sku_code**

Subscription SKU code, separated by comma. Recharge reports a lot of empty data in this field.

**onepetdata_number_of_subs**

Total number of subs ever started by this customer.

**onepetdata_number_of_active_subs**

Number of active subscriptions at present.

## List of Inactive Subscribers

Name of list in Klaviyo: **onepetdata_Inactive Subscribers**

Klaviyo list ID: [ ]( )

### Definition

Customers with no active subscription. Updated every 2 hours.  

### Attributes

```
! Debugging in process - attributes are not reliable.

! Known error : number of active subs is showing 1, should be zero. The product names, variants, sku code of the last active subscription are shown.
```

**onepetdata_number_of_subs**

Total number of subscriptions started by this customer.

## Lists by the duration of subscriptions

The following lists are created based on the number of times a subscription was charged.

Normally a subscription is charged every month. But there can be exceptions:
* The customer might skip a charge in a month
* The customer might use a 45 day shipping interval instead of the regular 30 days interval
* The customer might add an one time product to her subscription, increasing the number of charges

In short, number of charges is an indication of the customer value. The following lists will be used for addressing churns at each stage of subscription length.

|Charge count |List ID    |Name   |
|:------------|:----------|:------|
|1            |YmAiD9     |M1 Subs: Initial Purchase But Not Rebilled Yet |
|2            |WVdWBR     |M2 Subs: rebilled once - 2nd purchase |
|3            |W4s8TZ     |M3 Subs: rebilled twice - 3rd purchase |
|6|QQLZ6f|M7 Subs: billed 6 times - 7th purchase |
|12|RHsyHB|M13 Subs: billed 12 times - 1 yr completed
|18|Tx4WiN|M19 Subs: billed 18 times - 1.5 yr completed
|24|Yvyj8c|M25 Subs: billed 24 times - 2 yr completed
