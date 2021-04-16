---
title: Attribution Logic
nav_order: 5
---
# Attribution Logic

The same attribution logic is used across all One Pet web properties.

Every transaction is tagged with the following parameters-

1. `utm_source`
2. `utm_medium`
3. `utm_campaign`
4. `utm_adset`
5. `utm_content`
6. `utm_term`
7. `utm_affid`
8. `utm_subid` 
9. `utm_referrer` - This is not a UTM parameter, but the domain from which the user came.

## Last Touch Attribution Logic

This was implemented in Q2 2020.

When a user's session starts, does the user bring UTM parameters? 

If yes, update all UTMs in the cookie. 

If no, keep all existing UTM parameters.

Cookie life is 7 days. When a order is placed, UTM values from the cookie are saved along with the order ID using a server side post back. 

## First Touch Attribution Logic

Implemented in Q1 2021.

When a user's session starts, does the user have any cookie saved?

If yes, do nothing. 

If not, save all UTMs in the cookie.

Cookie life is 365 days. When a order is place, UTM values are saved with the order by appending `_firsttouch` at the end. For example, `utm_source_firsttouch`.

Attribution is saved on the orders. While orders are traceable all the way to channel and campaigns, users who are not customers are out of scope of this tracking. 
