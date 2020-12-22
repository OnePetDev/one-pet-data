---
title: Honest Paws Klaviyo lists
nav_order: 4
---
# Klaviyo lists

Klaviyo lists are sent from the One Pet Data Lake.

## List of Active Subscribers

Name of list in Klaviyo: **onepetdata_Active Subscribers**

Klaviyo list ID: [Xpb2La](https://www.klaviyo.com/list/Xpb2La/onepetdata_active-subscribers)

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

Klaviyo list ID: [SzJKPQ](https://www.klaviyo.com/list/SzJKPQ/onepetdata_inactive-subscribers)

### Definition

Customers who have started subscriptions before but no active subscriptions at present. Updated every 2 hours.  

### Attributes

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

## Lists by the duration of subscriptions

The following lists are created based on the number of times a subscription was charged.

Normally a subscription is charged every month. But there can be exceptions:
* The customer may skip a charge in a month
* The customer may use a 45 day shipping interval instead of the regular 30 days interval
* The customer may add an one time product to her subscription, increasing the number of charges

While charge count is not the perfect measure of subscription length, it is the best indication of the customer value. The following lists will be used for addressing churns at each stage of subscription length.

|Charge count |List ID    |Name   |
|:------------|:----------|:------|
|1            |[YmAiD9](https://www.klaviyo.com/list/YmAiD9/onepetdata_m1-subs-initial-purchase-but-not-have-been-rebilled-yet)     |M1 Subs: Initial Purchase But Not Rebilled Yet |
|2            |[WVdWBR](https://www.klaviyo.com/list/WVdWBR/onepetdata_m2-subs-rebilled-once-2nd-purchase)     |M2 Subs: rebilled once - 2nd purchase |
|3            |[W4s8TZ](https://www.klaviyo.com/list/W4s8TZ/onepetdata_m3-subs-rebilled-twice-3rd-purchase)     |M3 Subs: rebilled twice - 3rd purchase |
|6            |[QQLZ6f](https://www.klaviyo.com/list/QQLZ6f/onepetdata_m7-subs-billed-6-times-7th-purchase)|M7 Subs: billed 6 times - 7th purchase |
|12           |[RHsyHB](https://www.klaviyo.com/list/RHsyHB/onepetdata_m13-subs-billed-12-times-1-yr-completed)|M13 Subs: billed 12 times - 1 yr completed
|18           |[Tx4WiN](https://www.klaviyo.com/list/Tx4WiN/onepetdata_m19-subs-billed-18-times-15-yr-completed)|M19 Subs: billed 18 times - 1.5 yr completed
|24           |[Yvyj8c](https://www.klaviyo.com/list/Yvyj8c/onepetdata_m25-subs-billed-24-times-2-yr-completed)|M25 Subs: billed 24 times - 2 yr completed

---
```
Updated on Dec 22nd, 2020
```
