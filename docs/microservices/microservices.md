---
title: Microservices
nav_order: 5
---
# Microservices in Google Cloud
{: .no_toc }

Microservices run as Google Cloud Funcions triggered by  cron configured in the Google Cloud scheduler.

### Sending Active Subscribers from Recharge to klaviyo

Scheduler: adding_charge_count_to_recharge_subs_id  
Cron: 0 */2 * * * (America/Puerto_Rico)

### Sending Inactive Subscribers from Recharge to klaviyo

Scheduler: recharge_to_klaviyo_inactive_subscribers  
Cron: 15 */2 * * * (America/Puerto_Rico)

### Sending Recharge recharge count to Klaviyo lists

Scheduler: recharge_monthly_subs_to_klaviyo  
Cron: 0 6,18 * * * (America/Puerto_Rico)

### Getting charge count for recharge subscribers when they create an order

Scheduler: adding_charge_count_to_recharge_subs_id  
Cron: 0 6,18 * * * (America/Puerto_Rico)

---
```
This page is incomplete, as of Dec 22nd, 2020.
```
