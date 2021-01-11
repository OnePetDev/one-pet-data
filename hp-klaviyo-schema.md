---
title: Klaviyo Honest Paws
has_children: false
parent: Data Lake
nav_order: 1
---
# Klaviyo - Honest Paws
{: .no_toc }

We have 5 tables in Klaviyo, explaining 5 events that an email subscriber can accomplish.

- open
- receive
- click
- subscribe_list
- unsubscribe

Data in each table can be categorizes as either **event** properties or **person** properties.

#### Table of contents
{: .no_toc }

1. Table of contents
{:toc}

## Event Properties

These are the properties related to the events such as open, click and subscribe.

### receive

Data about users receiving emails.

* **campaign_name** - Name of the campaign [`Dog-HPNewsletter-01-07-21`], or in case of flows, name of the flow email [`03 | Abandoned cart Recharge | Email 4 | Testimonial`].
* **subject** - Subject line.
* **timestamp** - The time of receiving email, in epoch format.
* **_flow** - The unique Flow ID that is present on Klaviyo flow URLs. For example, `S9tX9V`. This is `null` for campaigns.
* **_message** - The unique ID for email. For example, `VbVYYT`.
* **_variation** - The ID for variation when an AB test is used. For example, `VKrMX2`.

### open

Data about users opening emails.

* **campaign_name** - Name of the campaign [`Dog-HPNewsletter-01-07-21`], or in case of flows, name of the flow email [`03 | Abandoned cart Recharge | Email 4 | Testimonial`].
* **subject** - Subject line.
* **timestamp** - The time of opening email, in epoch format.
* **_flow** - The unique Flow ID that is present on Klaviyo flow URLs. For example, `S9tX9V`. This is `null` for campaigns.
* **_message_interaction** - The unique ID for email. For example, `VbVYYT`.
* **_variation** - The ID for variation when an AB test is used. For example, `VKrMX2`.

### click

Data about users clicking on email links.

* **campaign_name** - Name of the campaign [`Dog-HPNewsletter-01-07-21`], or in case of flows, name of the flow email [`03 | Abandoned cart Recharge | Email 4 | Testimonial`].
* **subject** - Subject line.
* **timestamp** - The time of clicking, in epoch format.
* **_flow** - The unique Flow ID that is present on Klaviyo flow URLs. For example, `S9tX9V`. This is `null` for campaigns.
* **_message** - The unique ID for email. For example, `VbVYYT`.
* **_variation** - The ID for variation when an AB test is used. For example, `VKrMX2`.
* **url** - The clicked URL

### subscribe_list

Data when a user is subscribed to a list.

* **list** - Name of the list, for example `Master List`.
* **timestamp** - The time of clicking, in epoch format.

### unsubscribe

Data when a user is unsubscribed.

* **campaign_name** - Name of the campaign [`Dog-HPNewsletter-01-07-21`], or in case of flows, name of the flow email [`03 | Abandoned cart Recharge | Email 4 | Testimonial`].
* **subject** - Subject line.
* **timestamp** - The time of clicking, in epoch format.
* **_flow** - The unique Flow ID that is present on Klaviyo flow URLs. For example, `S9tX9V`. This is `null` for campaigns.
* **_message** - The unique ID for email. For example, `VbVYYT`.
* **_variation** - The ID for variation when an AB test is used. For example, `VKrMX2`.

Additionally, we have data on the user's device, browser and operating system for each of the above events.

## Person

The attributes associated with a person are listed below. Not everyone has all the data points.

*  recommended_product_url_1			
*  recommended_product_image_2			
*  recommended_product_image_3			
*  recharge_subscription			
*  object			
*  wsegment			
*  _country			
*  referral_friend_offer___referralcandy			
*  created			
*  _longitude			
*  _longitude__st			
*  _longitude__nu			
*  nps_comment			
*  _last_name			
*  pet_name			
*  _address2			
*  expected_date_of_next_order			
*  _consent			
* _consent. value			
*  recharge_honestpaws_active_subscribers_			
*  refer_link			
*  use_case			
* use_case. value			
*  drift			
*  referral_link_with_tracking___referralcandy			
*  nps_score			
*  recommended_product_url_3			
*  last_abandoned_product			
*  recommended_product_1			
*  birthday			
*  campaign_			
*  yotpo_latest_review_score			
*  phone_number			
*  _organization			
*  campaign_name			
*  _email			
*  recharge_subscriptions			
* recharge_subscriptions. value			
*  _carthook_funnel_id			
*  smile_vip_tier_name			
*  id			
*  _consent_form_id			
*  completed_welcome			
*  email			
*  _address1			
*  _phone_number			
*  _city			
*  do_you_use_nsaids_for_your_pet			
*  yotpo_crf_pet			
*  yotpo_number_of_reviews			
*  smile_referral_url			
*  initial_referring_url			
*  yotpo_crf_weight			
*  last_abandoned_image			
*  recommended_product_image_1			
*  does_your_dog_suffer_from_some_of_these_ailments			
*  _source			
*  _source__st			
*  pet_weight			
*  which_medication_has_your_pet_used			
*  shopify_tags			
* shopify_tags. value			
* shopify_tags. value__ar			
* shopify_tags.value__ar. value			
*  campaign			
*  recommended_product_url_2			
*  _consent_timestamp			
*  hidden__utm_source			
*  _first_name			
*  yotpo_crf_pet_s_birthday			
*  ip			
*  hidden__utm_content			
*  yotpo_crf_breed			
*  yotpo_crf_concern			
*  _latitude			
*  _latitude__st			
*  _latitude__nu			
*  referral_reward___referralcandy			
*  yotpo_crf_number_of_pets			
*  _consent_form_version			
*  _consent_form_version__it			
*  utm_source			
*  last_name			
*  utm_medium			
*  pet_type			
* pet_type. value			
* this_is_not_required__if_you_would_like_to_get_sms_notifications_for_other_special_offers__enter_your_mobile_number_below_			
*  first_name			
*  how_old_is_your_pet			
*  referral_portal_link___referralcandy			
*  smile_points_balance			
*  source			
*  yotpo_crf_pet_name			
*  discount_code			
*  is_your_pet_on_any_medication			
*  recommended_product_2			
*  utm_campaign			
*  recharge_honestpaws_inactive_subscribers_			
*  shopping_for			
*  _id			
*  _consent_method			
*  what_type_of_animals_do_you_have			
*  _region			
*  updated			
*  accepts_sms			
*  yotpo_last_email_sent			
*  source_name			
*  ip_address			
*  hidden__utm_medium			
*  accepts_marketing			
*  accepts_marketing__st			
*  _zip			
*  _timezone			
*  hidden__utm_campaign			
*  _title			
*  does_your_pet_suffer_from_any_health_issues			
*  variant			
*  recommended_product_3			
*  referral_link___referralcandy			
*  smile_state			
*  smile_vip_tier_id			
*  source_			
*  last_ordered_image			
*  how_much_does_your_pet_weight_			
*  pet_breed			
*  confirm_optin			
*  lytics_audience			
*  gender			
*  does_your_dog_suffer_from_some_or_these_ailments			
*  last_ordered_product			
*  last_ordered_url			
*  pet_type__st			
*  how_many_pets_do_you_have			
*  lytics_honestpaws_repeat_customers_not_subscribers_			
*  trial_product			
*  dog_type			
*  checkout_url			
*  use_case__st			
*  dog_name			
*  utm_content			
*  recharge_zapier_subscription			
*  recharge_zap_status			
*  _id__it			
*  how_much_does_your_pet_weigh_			
*  _list			
*  _listi			
*  _listid			
*  product_inquired			
*  _method_type			
*  _method_id			
*  _consent_version			
*  recharge_customer			
*  auto_refill			
*  entered_sweepstakes			
*  onepetdata_number_of_subs			
*  onepetdata_number_of_subs__st			
*  rc_active_subscriber			
*  onepetdata_subs_variant_name			
*  onepetdata_number_of_active_subs			
*  onepetdata_subs_sku_code			
*  onepetdata_subs_product_name			
*  onepetdata_subs_start_dates			
*  subscriber_free_product			
*  rc_queued_charge_count			
* datetime

---
```
This page is updated on Jan 11th, 2021.
```
