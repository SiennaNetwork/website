---
_archived: false
_draft: false
featured: false
published-date-month: "May"
name: "SiennaLend Update"
published-date-2: "13"
read-time-in-min: "3 min."
post-summary: "sUST/sLUNA Markets Postmortem + Liquidation Bot is Live"
slug: "siennalend-update"
thumbnail-image:
  url: "https://uploads-ssl.webflow.com/60621456954600aa473c3cd0/629506e66b080304c70e0e49_SiennaLend%20Update%20Blog%20Thump.jpg"
  alt: ""
main-image:
  url: "https://uploads-ssl.webflow.com/60621456954600aa473c3cd0/629506e22bc70cbb65eefb56_SiennaLend%20Update%20Blog.jpg"
  alt: ""
updated-on: "2022-05-30T18:03:50.396Z"
created-on: "2022-05-30T18:03:50.396Z"
published-on: "2022-05-30T18:03:50.396Z"
tags: "blog"
layout: "single-blog.html"
---

#### SiennaLend Update: sUST/sLUNA Markets Postmortem + Liquidation Bot is Live

##### With UST losing its peg and the LUNA price dipping to oblivion, the whole Cosmos DeFi ecosystem suffered from the ensuing snowball effect. SiennaLend faced issues with rapidly increasing bad debt, which we managed to limit so that exposed users do not suffer losses.

##### SiennaLend sUST/sLUNA Markets Postmortem

‍

#### Sequence of Events

*   UST loses its peg and LUNA price deteriorates rapidly (Thursday, May 12, 2022).
*   Binance delists LUNA and UST pairs ( Friday, May 13, 2022).
*   Oracle provider stops providing price feeds for UST and LUNA without notice (Friday, May 13, 2022 4:36 AM).

‍

#### **This results in a scenario similar to oracle manipulation:**

1.  Users who had entered UST and/or LUNA markets are not able to use SiennaLend.
2.  Oracle returns errors instead of 0 as value for LUNA and UST which rendered the liquidation bot useless as it could not query the markets.

*   Investigation of side-effects and possible damage to the product and users ( Friday, May 13, 2022 8:12 AM).

‍

#### **Internal discussion on possible ways forward:**

(Friday, May 13, 2022 9:42 AM).

*   Simulate system behaviour with price for sUST and sLuna set to 0

**Oracle fix:**

1.  Option 1: ask oracle provider to provide 0 instead of the errors they throw, so that the operations resume for other markets.
2.  Option 2: deploy new oracle consumer which ignores Error messages from oracle provider’s UST and Luna feeds.

*   Subsidized rewards for sUST and sLUNA SiennaSwap pairs/SiennaLend markets are redistributed to other pairs/markets (Friday, May 13, 2022 3:57 PM).

Started work on Option 2 ( Friday, May 13, 2022 5:20 PM).

*   New Oracle Consumer (with the oracle provider error handling fix) is uploaded (Friday, May 13, 2022 6:00 PM).
*   New Oracle Consumer Instantiated ( Friday, May 13, 2022 6:04 PM).
*   Compared query results from old and new one ( Friday, May 13, 2022 6:08 PM).
*   Prepped tx for Oracle Consumer change in the Overseer contract (Friday, May 13, 2022 6:08 PM).
*   Band Protocol agreed to send real prices for 1HR so LTV ratios for the failed markets can be set to 0 (Friday, May 13, 2022 6:53 PM).
*   Changed LTV ratio to 0 for sUST and sLUNA markets (Friday, May 13, 2022 6:54 PM).
*   Switched to new Oracle Consumer (Friday, May 13, 2022 7:31 PM).

‍

#### sLUNA & sUST Bad Debt was Covered by Sienna Contributors

As a gesture of good faith and our unyielding commitment to the Sienna Network community, the sLUNA and sUST bad debts that accumulated as a result of the Terra collapse were covered by core contributors to Sienna Network. ❤️

This prevented a mass liquidation event that would have hurt a large portion of SiennaLend users.

‍

#### SiennaLend Liquidation Bot is Live

Liquidation bots monitor open loans and check for positions that are eligible for liquidation (loans are liquidated when the risk ratio is at or above 100%). The SiennaLend liquidation bot is now live. Users can follow the instructions outlined below to create their own:

[https://github.com/SiennaNetwork/lend-liquidation-bot](https://github.com/SiennaNetwork/lend-liquidation-bot)
