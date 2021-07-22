---
title: Subscription Gifts
nav_order: 7
---
# Subscription Gifts for Recharge
{: .no_toc }

This app lets us send gifts to subscribers based on the month of subscription.

It checks for recent orders that are subscription recurring charges, and checks which month they are in. It selects the orders which are in their second [or, any] month, and creates orders in recharge and shopify for those customers.

The program relies on shopify order tags containing "Subscription Recurring Order" to identify the orders. Additionally, it works on subscriptions that started with the "Auto Refill Free Shipping" shipping code, otherwise the gift would add a shipping charge set in shopify. 

For detailed specifications, visit [click up story](https://app.clickup.com/t/8599650/DATA-229) or [github repo](https://github.com/OnePetDev/data-cloud-functions/tree/master/07_free_gift_on_auto_refill_orders)

The function runs on [Google Cloud Functions](https://console.cloud.google.com/functions/details/us-central1/recharge_subs_gifts?project=one-pet-data-lake), triggered by a Cloud scheduler cron job, `recharge_create_subscription_gift_m2`. 
