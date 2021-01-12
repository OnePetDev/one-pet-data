---
title: Recharge Honest Paws
has_children: true
parent: Data Schema
nav_order: 2
---
# Recharge - Honest Paws
{: .no_toc }

Data in recharge is abstracted in four key objects - Subscriptions, Customers, Addresses and Orders.

![](../../assets/images/recharge-subscriptions.png)

An order is created after a charge is successfully processed. The order contains all the same json data as the charge. In case of a prepaid order creation, the order will be queued for a particular date and submitted on that date to shopify.

![](../../assets/images/recharge-order.png)

---
```
This page is updated on Jan 11th, 2021.
```
