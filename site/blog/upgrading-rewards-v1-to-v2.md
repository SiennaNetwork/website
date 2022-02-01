---
_archived: false
_draft: false
featured: false
published-date-month: "October 2021"
name: "Upgrading Rewards V1 to V2"
published-date-2: "16"
read-time-in-min: "2 min."
post-summary: "During the launch everything was double checked but an unintended “feature” came to light right after launching."
thumbnail-image:
  url: "https://uploads-ssl.webflow.com/60621456954600aa473c3cd0/616d39f2e4778a84184efca4_SiennaSwap%20Update%20Rewards%20Blog%20Thump.jpg"
  alt: ""
main-image:
  url: "https://uploads-ssl.webflow.com/60621456954600aa473c3cd0/616d39f5234cff083ec3703b_SiennaSwap%20Update%20Rewards%20Blog.jpg"
  alt: ""
slug: "upgrading-rewards-v1-to-v2"
updated-on: "2022-01-10T09:51:15.267Z"
created-on: "2021-10-18T09:10:27.610Z"
published-on: "2022-01-10T09:51:15.267Z"
tags: "blog"
layout: "single-blog.html"
---

SiennaSwap launched October 7th along with attractive rewards for liquidity mining, which is an essential part of attracting liquidity to AMMs and the like.  
However, the rewards were a little more attractive than intended. Actually 159 times more attractive than what was planned. Here is how it happened and what was done to fix it.

The rewards pool accounts for a whopping 36% of all SIENNA, meaning 3,600,000 in total. The daily allocation is 2,500 SIENNA and they are distributed to the different pools in order to reward the liquidity providers. Users can claim earned rewards every 12500 blocks (~23 hours) and your earnings will largely depend on your share of the pool.

During the launch everything was double checked but an unintended “feature” came to light right after launching. Extraordinarily high rewards for the first 24 hours were about to be released. Instead of 2,500 SIENNA it would amount to 397,500 the first day. How could this happen? Here is how.

When the token generation event happened on May 2nd, 2021 the minting pool was also generated as part of the total 10,000,000 SIENNA. The rewards were ready to be allocated on a daily basis to the rewards contract. This means that the rewards contract have been acting as intended and receiving 2500 tokens per day since May 2nd, which at the time of SiennaSwap’s launch was 159 days ago, meaning 159 times the amount of rewards the first day at launch, which was an oversight during mainnet deployment in the haste of things, since all testnet deployments started from the same date.

The impact was that those few users that got to claim before the rewards contracts were paused via a multisig and was migrated to V2 quickly after, got lucky. The total amount of rewards that was distributed in this way was~20,000 SIENNA.

Additionally, to make up for this, 20,000 SIENNA tokens will (once vested) come out of the development fund to make up for the 8 days “lost” in liquidity mining. And finally, rewards V2 were boosted to 3x for the first 24 hours to make up for the missed 2–3 days during the migration.

Thanks to the community for their understanding and swift feedback.

Happy private swapping!

‍
