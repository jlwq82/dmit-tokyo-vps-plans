# DMIT Tokyo VPS: Which Line Do You Need, What It Costs, and Does Annual Billing Save Anything? (All 19 Plans Compared)

DMIT sells three separate Tokyo products, and they are not three grades of the same server. **Pro** starts at **$21.90/month** and sends return traffic over China Telecom's CN2 GIA. **Eyeball (EB)** starts at **$25.90/month**, uses CMI for the return path and gives you far more bandwidth. **Tier 1 (T1)** starts at **$6.90/month**, or **$36.90/year** on the WEE plan, with no mainland China optimisation at all.

Pick by your ISP and your bandwidth needs. The cheapest plan is not the entry point to the premium network, and the premium network is not the most expensive entry plan.

## Quick pick

- **Most people comparing Tokyo VPS for China access:** TYO.Pro.TINY, $21.90/month, 1 vCPU / 1GB / 20GB / 500GB at 1Gbps.
- **You just need a Japan IP or serve users in Japan and East Asia:** TYO.T1.TINY at $6.90/month, or WEE at $36.90/year if 1TB is enough.
- **You are on China Mobile and want 2 to 4Gbps:** TYO.EB, but confirm stock before you plan around it.

👉 [Check current Tokyo plans and stock at DMIT](https://www.dmit.io/aff.php?aff=9081)

## What actually separates Pro, EB and T1

The difference is the return path, meaning how traffic comes back from Tokyo to your ISP in China.

**Pro (TYO.AS3.Pro)** returns all three networks over CN2 GIA. Outbound, Telecom and Unicom take premium routes and Mobile goes over CMI. Published third-party tests put Tokyo to Beijing at roughly 60 to 65ms for Telecom and 50 to 55ms for Unicom and Mobile, holding steady at peak hours. This is the line you buy when latency and packet loss are the whole point.

**EB (TYO.AS3.EB)** returns over CMI. Traffic leaves the server, crosses DMIT's own backbone (AS906), hands off to CMI's Japan node (AS58453), lands in Shanghai and then spreads out nationally. Mobile traffic takes the most direct version of that path at 55 to 65ms. Telecom and Unicom traffic goes CMI into China Mobile's domestic network and then back to its own, which is why Telecom return tests run 58 to 80ms instead of Pro's 60 to 65ms. You will see EB described as "CMIN2" in some affiliate write-ups. The published route traces show an AS906 to AS58453 handoff, so CMI is the accurate label.

**T1 (TYO.AS3.T1)** is a plain international line. Telecom and Unicom route over NTT, Mobile over CMI or Lumen. Nothing is optimised for mainland China. What you get instead is bandwidth (4Gbps at entry, 10Gbps from STARTER up) and a much lower price.

Here is the counterintuitive part: **Pro's entry plan is cheaper than EB's**, $21.90 against $25.90. EB is not a downgrade in price, it is a different product. EB sells port speed and monthly traffic. At the same 1 vCPU / 1GB / 20GB spec, EB gives you 1TB instead of Pro's 500GB, and EB scales to 4Gbps where Pro stays at 1Gbps across the entire range.

## All Tokyo plans and prices

Prices in USD. Traffic is monthly. Over-quota behaviour is covered further down.

### TYO.Pro (CN2 GIA return)

| Plan | vCPU / RAM / SSD | Traffic / Port | Monthly | Annual | Order |
| --- | --- | --- | --- | --- | --- |
| TINY | 1 / 1GB / 20GB | 500GB / 1Gbps | $21.90 | $262 | [TYO.Pro.TINY](https://www.dmit.io/aff.php?aff=9081) |
| STARTER | 1 / 2GB / 40GB | 1000GB / 1Gbps | $39.90 | $478 | [TYO.Pro.STARTER](https://www.dmit.io/aff.php?aff=9081) |
| MINI | 2 / 2GB / 60GB | 2000GB / 1Gbps | $79.90 | $958 | [TYO.Pro.MINI](https://www.dmit.io/aff.php?aff=9081) |
| MICRO | 4 / 4GB / 80GB | 4000GB / 1Gbps | $159.90 | $1,918 | [TYO.Pro.MICRO](https://www.dmit.io/aff.php?aff=9081) |
| MEDIUM | 4 / 8GB / 160GB | 5000GB / 1Gbps | $259.90 | $3,118 | [TYO.Pro.MEDIUM](https://www.dmit.io/aff.php?aff=9081) |
| LARGE | 8 / 16GB / 320GB | 8000GB / 1Gbps | $429.90 | $5,158 | [TYO.Pro.LARGE](https://www.dmit.io/aff.php?aff=9081) |
| GIANT | 8 / 24GB / 640GB | 15000GB / 1Gbps | $799.90 | $9,598 | [TYO.Pro.GIANT](https://www.dmit.io/aff.php?aff=9081) |

### TYO.EB (CMI return, up to 4Gbps)

| Plan | vCPU / RAM / SSD | Traffic / Port | Monthly | Annual | Order |
| --- | --- | --- | --- | --- | --- |
| EB.TINY | 1 / 1GB / 20GB | 1000GB / 1Gbps | $25.90 | $310 | [TYO.EB.TINY](https://www.dmit.io/aff.php?aff=9081) |
| EB.STARTER | 1 / 2GB / 40GB | 2000GB / 2Gbps | $55.90 | $670 | [TYO.EB.STARTER](https://www.dmit.io/aff.php?aff=9081) |
| EB.MINI | 2 / 2GB / 60GB | 3000GB / 2Gbps | $85.90 | $1,030 | [TYO.EB.MINI](https://www.dmit.io/aff.php?aff=9081) |
| EB.MICRO | 4 / 4GB / 80GB | 4000GB / 4Gbps | $119.90 | $1,438 | [TYO.EB.MICRO](https://www.dmit.io/aff.php?aff=9081) |
| EB.MEDIUM | 4 / 8GB / 160GB | 6000GB / 4Gbps | $179.90 | $2,158 | [TYO.EB.MEDIUM](https://www.dmit.io/aff.php?aff=9081) |
| EB.LARGE | 8 / 16GB / 320GB | 12000GB / 4Gbps | $369.90 | $4,438 | [TYO.EB.LARGE](https://www.dmit.io/aff.php?aff=9081) |
| EB.GIANT | 8 / 24GB / 640GB | 24000GB / 4Gbps | $749.90 | $8,998 | [TYO.EB.GIANT](https://www.dmit.io/aff.php?aff=9081) |

### TYO.T1 (international, no China optimisation)

| Plan | vCPU / RAM / SSD | Traffic / Port | Monthly | Annual | Order |
| --- | --- | --- | --- | --- | --- |
| WEE | 1 / 1GB / 20GB | 1000GB / 4Gbps | not offered | $36.90 | [TYO.T1.WEE](https://www.dmit.io/aff.php?aff=9081) |
| TINY | 1 / 1GB / 20GB | 2000GB / 4Gbps | $6.90 | $76.90 | [TYO.T1.TINY](https://www.dmit.io/aff.php?aff=9081) |
| STARTER | 1 / 2GB / 40GB | 4000GB / 10Gbps | $12.90 | $154.80 | [TYO.T1.STARTER](https://www.dmit.io/aff.php?aff=9081) |
| MINI | 2 / 2GB / 60GB | 8000GB / 10Gbps | $21.90 | $262.80 | [TYO.T1.MINI](https://www.dmit.io/aff.php?aff=9081) |
| MICRO | 4 / 4GB / 80GB | 16000GB / 10Gbps | $32.90 | not listed | [TYO.T1.MICRO](https://www.dmit.io/aff.php?aff=9081) |

All three lines run AMD EPYC 7003 series CPUs (EPYC 7443P on some nodes), KVM virtualisation, enterprise SSD, one IPv4 plus one IPv6 /64, and AES-NI. Prices and stock are what was listed when this was written; the order page is the only place that is current.

## Annual billing saves almost nothing. Check the numbers before you commit.

Most Tokyo VPS reviews say annual billing is cheaper. Run the arithmetic on this specific price list and that claim mostly falls apart.

- T1.TINY: $6.90 × 12 = $82.80. Annual is $76.90. You save $5.90, about 7%.
- T1.STARTER: $12.90 × 12 = $154.80. Annual is $154.80. **Zero difference.**
- T1.MINI: $21.90 × 12 = $262.80. Annual is $262.80. **Zero difference.**
- Pro.TINY: $262.80 monthly, $262 annual. Saves $0.80.
- EB.TINY: $310.80 monthly, $310 annual. Saves $0.80.

At that level, paying a year up front buys you nothing except exposure. Start monthly, run your own latency and throughput tests for a couple of weeks, and only then decide whether the plan you picked is the plan you want. The 3-day refund window is enough to confirm the server boots and routes correctly, not enough to judge peak-hour behaviour across a billing cycle.

The one route to a real discount is a working recurring coupon on quarterly or longer terms, which is worth testing at checkout given that it can cut 20 to 30% off the renewal price rather than just the first invoice.

## Limits that matter more than the spec sheet

**Traffic overage.** Pro and EB suspend service when you exceed the monthly allowance. You pay to restore it. T1 throttles instead, dropping to roughly 50Mbps (some sources say 50 to 100Mbps) and keeps running without a hard stop. If your workload is bursty or you would rather be slow than offline, this single difference matters more than the CPU.

**Free IP replacement covers Pro and EB only.** If the IP gets blocked by the GFW, Pro and EB customers can request a replacement free of charge, once every 15 days. Changes for any other reason cost $5. T1 is outside this policy, so a T1 buyer whose IP gets blocked has no free path back. Factor that into the $6.90/month calculation if you are using the server for anything that attracts blocking.

**Refunds.** Full refund within 3 days of purchase if you have used no more than 30GB of traffic, minus the payment gateway fee. Between day 3 and day 30, refunds are prorated by remaining service time. Refunds to account balance carry no fee; refunds to the original payment method lose the gateway fee. Renewal orders, orders paid from account balance, a third refund on the same product line, and IP-blocked cases are not refundable.

**Login is SSH key only.** There is no root password. The key is in the welcome email or under the Networking section of the control panel. New users sometimes open a ticket thinking the server is broken when they simply have not downloaded the key yet.

👉 [Start with a monthly TYO.Pro.TINY and test the route yourself](https://www.dmit.io/aff.php?aff=9081)

## Who should buy which

**Telecom user, latency sensitive, running a game server, a relay or anything where 10ms and packet loss matter:** Pro. TYO.Pro.TINY at $21.90/month is the cheapest way into CN2 GIA return from Tokyo, and the Hong Kong equivalent starts at $39.90/month for the same TINY spec. Tokyo adds roughly 5 to 30ms over Hong Kong (Hong Kong tests under 50ms to major Chinese cities; Tokyo runs 55 to 80ms) and costs about half as much.

**China Mobile user who wants bandwidth:** EB. On Mobile the EB path is the most direct of the three and the 2 to 4Gbps ports are not something Pro offers at any price. On Telecom, EB's return path is a step down from Pro and the 58 to 80ms figures show it.

**Serving users in Japan, Korea or Southeast Asia, or you just need a Japanese IP:** T1. $6.90/month or $36.90/year, 4Gbps at entry, throttled rather than suspended on overage. A small blog, a monitoring node or a lightweight proxy does not need CN2 GIA return, and the extra $15/month that Pro costs over T1.TINY buys routing quality you will not notice.

**Willing to pay for the lowest possible latency:** Hong Kong Premium, if it is in stock. It is faster and more expensive, and its stock is tighter than Tokyo's. That is the whole trade.

**Who should not buy here at all:** anyone whose main requirement is the cheapest possible Japan IP with no interest in China routing. T1 is fine, but DMIT's pricing is built around network quality, and the $6.90 plan is the edge of what it offers, not its strength.

## EB stock and coupon codes: read this before checkout

Community sources from March and April 2026 reported the TYO EB series as delisted or out of stock on the official site, with Pro restocked but tight and T1 available. That information is now about seven months old and cannot be treated as current. Check the order page for the EB plans before you build a plan around them.

On coupons, the circulating codes are from 2025 promotions and may well be expired:

- `2025-TYO-T1-HI-GSL-MONTHLY-10OFF` for 10% off T1 monthly
- `2025-TYO-T1-HI-GSL-NON-MONTHLY-30OFF` for 30% off T1 quarterly and longer, recurring
- `202510_HKG_TYO_PRO_20OFF_RECURRING` for 20% off Pro (Tokyo and Hong Kong) quarterly and longer, recurring

Nothing applies automatically. Enter the code in the promo code field on the checkout page and watch whether the total actually changes. An expired code produces no discount and no error message worth reading. If the 30% T1 code is still live, it changes the annual-billing math above completely, which is the main reason to try it before defaulting to monthly.

## FAQ

**Can DMIT Tokyo unlock streaming services?**
Every plan includes a native IP. Users have reported Netflix Japan and TikTok working on some assignments. Abema, Hulu Japan and other domestic platforms are not guaranteed, and DMIT does not market streaming unlocks as a feature. Test on a monthly plan before committing if this is your main use.

**Is DMIT oversold?**
DMIT states that it does not oversell, and long-term user reports describe consistent peak-hour performance. There is no independent measurement to prove a negative here, so treat it as the vendor's claim backed by community observation rather than a verified fact.

**Tokyo or Hong Kong?**
Hong Kong wins on latency, under 50ms to major Chinese cities against Tokyo's 55 to 80ms. Tokyo wins on price and availability, with Pro TINY at $21.90/month against Hong Kong Pro TINY at $39.90/month and far tighter stock. If you need the absolute lowest latency and can pay for it, Hong Kong. If you want CN2 GIA return at a reasonable price, Tokyo.

**How do I pay?**
USD billing, with Alipay, WeChat Pay and PayPal accepted. Support is available in Chinese, which matters if you need to sort out a routing issue at 2am.

**What happens if I outgrow the plan?**
DMIT handles upgrades and downgrades through support tickets. Plan your RAM and disk with some headroom, since Tokyo plan prices step up steeply between tiers.

## Before you order

Match the line to your ISP first, then the plan size to your workload. Telecom and latency-critical goes to Pro. Mobile and bandwidth-hungry goes to EB, subject to stock. Japan-facing or IP-only goes to T1, and TINY at $6.90/month or WEE at $36.90/year is enough for that job.

Then confirm two things on the order page: that the plan you want is actually in stock, and whether your coupon code reduces the total. Both change without notice, and neither is something a review written months ago can tell you.

👉 [Compare DMIT Tokyo plans, prices and live stock](https://www.dmit.io/aff.php?aff=9081)
