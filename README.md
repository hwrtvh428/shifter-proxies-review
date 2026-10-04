# Shifter Proxies Review: What $0.75/GB Buys You, Where the Old Port Plans Went, and a Cheaper Per-GB Alternative

Most people searching for a Shifter review are in one of two situations. Either they still have a MicroLeaves account sitting around from years back and want to know what happened to it, or they're running a scraping bill that's crept past what they expected to pay per gigabyte. The two situations lead to the same place, and both run into the same problem: the brand has changed names twice, changed its billing model once, and most of the pages ranking for its name were written before either happened.

So this is a review written against what the vendor publishes now, plus what third-party directories have measured, plus the one thing that actually decides whether Shifter is worth your money — the per-gigabyte math at your volume.

## What Shifter is today, and why the name keeps changing

Shifter has been in the proxy business since 2012. It started as reverseproxies.com, rebranded to MicroLeaves, and now trades as Shifter. That history matters to buyers because the old MicroLeaves domain is still online and still confusing: one directory review of the legacy site notes a copyright notice from 2016, pricing and proxy sub-pages that return 404 errors, and a redirect pointing visitors to Shifter.io. If you land on a page that looks like it was built a decade ago and quotes $12.50/GB, you're reading the dead version of the company.

What the current brand sells is residential rotating proxies as the main product, with static residential and ISP proxies alongside, plus datacenter options in the older backconnect/dedicated/shared framing that still circulates in comparison tables. The cheapest datacenter-tier references floating around describe plans in the hundreds of ports rather than gigabytes.

Where third-party directories disagree, and they do, is on the company's location — the New York and United Kingdom labels both show up. That's a small thing, but it's the kind of small thing worth noticing when a vendor's own sub-pages are broken.

The current product, per the vendor's own announcement:

- one gateway for everything, so country, session and targeting parameters live in the username string instead of separate endpoints per plan
- **205M+ residential IPs across 195+ countries** (advertised)
- bandwidth-based billing on all plans, replacing port allocations
- city and ASN targeting included on every tier, with no premium
- no concurrency or request-rate caps, since you're billed on data rather than ports

## Shifter pricing: two eras in one product

This is where most reviews go wrong, because two pricing models circulate for the same brand.

Here's the current bandwidth table, as published by the vendor:

| Plan | Traffic | Rate per GB | Monthly cost |
| --- | --- | --- | --- |
| Entry | 5 GB | $2.00 | $10 |
| Starter | 50 GB | $1.00 | $50 |
| Basic | 100 GB | $1.00 | $100 |
| Business | 200 GB | $0.75 | $149 |
| Growth | 400 GB | $0.75 | $299 |

The best published rate is **$0.75/GB from 200 GB up**, and every tier is public — no sales call required to see the number, which is not true of every provider in this bracket.

The other era is port-based. Older listings still quote plans like $299.99 for 25 ports with unmetered traffic, and that was the actual product for years. The vendor now says customers on port plans can ask support to pull their usage history and work out the bandwidth-equivalent package. If you're on a legacy plan, that's the conversation to have before you buy anything new.

Two practical limits on the pricing:

- There's **no free trial**. The money-back window is roughly 72 hours according to directory listings, which is a very short window for a workload that takes weeks to evaluate.
- The 5 GB entry tier prices at $2.00/GB. If your volume lands under 50 GB a month, you're paying four times the rate a mid-volume buyer pays. That tier exists to let you test the gateway, not to run production.

## Performance: whose numbers are you actually reading?

Shifter runs what it calls benchmarks against named competitors, published on its own domain. The method is stated clearly enough to be worth summarising: 250,000 requests per provider, concurrency of 1,000, a 10-second timeout, one provider at a time on a single machine so they don't compete for bandwidth, with each request opening a fresh connection so the exit address count reflects reachable IPs rather than advertised pool size.

The headline results from those runs: **136,667 live US IPs, 1,606 distinct networks, 5,813 cities, 364 ms average latency and a 99.8% success rate.**

Those are vendor numbers on a vendor domain, testing competitors. They're not worthless — the methodology is specific and the failure numbers are published too — but they're a claim, not an audit.

The independent-ish picture looks different, and less flattering in places:

- One proxy directory lists Shifter at **3.8/5 overall with a 6.8/10 trust score**, and separately cites 98.43% success and 880 ms average response from its own benchmark data.
- Another directory scores it **4.8/5** and, in a listing that appears not to have been refreshed, says city-level geotargeting isn't available — which contradicts the vendor's city targeting claim directly. That contradiction is a good reason to verify targeting on the specific city you need before committing to a large package.
- The same directory lists a **72-hour money-back period** and notes the product isn't suited to users who only need a small amount of traffic.
- One review site publishes a split verdict of **7.1/10 from its own testing against 1.7/10 from user submissions**, with the complaints concentrated on customer support, connection errors and the absence of a free trial.
- Trustpilot coverage is thin enough to be useless: a score around 2.9/5 built on two reviews tells you nothing about the product.

Read together, the pattern is: a large advertised pool, a genuinely competitive published rate card, and a public evidence base that is too sparse and too contradictory to settle whether the network is fast. The 205M+ figure is advertised, not measured; one directory sampled roughly 235,000 live addresses. Residential IPs rotate constantly, so that gap is expected, but it also means pool size shouldn't be the thing you decide on.

## Where Shifter is a reasonable buy, and where it isn't

It's a reasonable buy if your work is bandwidth-heavy and the proxy bill is the line item you're trying to cut. At $0.75/GB and everything public, the arithmetic is easy to run: 100 GB of residential traffic costs $100, and the tier below the best rate is only $1.00/GB. City and ASN targeting being included on every tier rather than gated behind enterprise contracts matters more than it sounds — ad verification and local price monitoring both break without it.

It's a poor fit if you want to test before paying, if your volume sits in the single-digit or low-double-digit gigabytes per month, or if you need hard independent proof of speed. The support complaints and the short refund window compound each other: you cannot test slowly and you cannot easily get your money back if it doesn't work.

A second consideration: Shifter's core identity is residential. If you need residential, mobile and datacenter from one dashboard and one invoice, a specialist residential-only provider won't help you there either, but at least you won't be paying residential rates for traffic a cheaper datacenter IP could carry.

## The cheaper unit: what 9Proxy actually charges

9Proxy runs in the opposite direction from Shifter. It's newer, it only does residential, and instead of one billing model it sells two — which is the part most reviews skip and the part that decides what you pay.

**Residential by IP:** you buy a fixed number of IPs and get unlimited bandwidth while each IP is active. Unused IPs don't expire. The catch is that each residential IP stays usable for a few hours up to about 24 hours, and this mode requires the desktop app with local port forwarding.

**Residential by GB:** you buy a traffic allowance and generate as many endpoints as you like. Country, state, city, ZIP and ISP targeting, sticky or rotating sessions, username/password or IP whitelist authentication, all handled in the dashboard with no app. Validity runs 180 days, or unlimited on Enterprise.

Here's the full rate card as published and reported across its documentation and partner guides:

| Plan | Model | Price | Rate | Validity |
| --- | --- | --- | --- | --- |
| 5 GB | Pay per GB | $15 | $3.00/GB | 180 days |
| 50 GB (+5 GB bonus) | Pay per GB | $105 | $2.10/GB | 180 days |
| 100 GB | Pay per GB | $150 | $1.50/GB | 180 days |
| 200 GB | Pay per GB | $200 | $1.00/GB | 180 days |
| 1,000 GB | Pay per GB | $800 | $0.80/GB | 180 days |
| 2,000 GB | Pay per GB | $1,500 | $0.75/GB | 180 days |
| 3,000 GB | Enterprise | $2,160 | $0.72/GB | No expiry |
| 6,000 GB | Enterprise | $4,200 | $0.70/GB | No expiry |
| 10,000 GB | Enterprise | $6,800 | $0.68/GB | No expiry |
| 100 IPs | Pay per IP | $24 | $0.24/IP | Bandwidth unlimited |
| 500 IPs | Pay per IP | $72 | $0.14/IP | Bandwidth unlimited |
| 1,000 IPs (+500 bonus) | Pay per IP | $126 | $0.08/IP | Bandwidth unlimited |
| 100,000 IPs | Pay per IP | $2,300 | $0.02/IP | Bandwidth unlimited |
| 500,000 IPs | Pay per IP | $8,625 | ~$0.017/IP | Bandwidth unlimited |

Bundle packages that combine a block of IPs with a traffic allowance also exist — commonly advertised around 100 IPs + 5 GB, 1,500 IPs + 50 GB and 5,000 IPs + 500 GB — but the quoted prices for these move more than the standard tiers, and published figures vary between sources, so check the current number rather than trusting a screenshot.

Two honest notes on the table. The vendor markets "from $0.015/IP"; the arithmetic at the top published IP tier lands closer to $0.017/IP, and at the smallest tier you're paying $0.24/IP. And on targeting, 9Proxy's own documentation lists city, ZIP and ISP level selection, while one third-party cost comparison describes its city-level targeting as limited. Both can be true — country coverage is 90+ countries, half of Shifter's advertised footprint — so test the specific location you need before scaling up.

Third-party positioning puts 9Proxy in the budget tier of the market, around the $0.70–$2/GB band, with Tier 1 and Tier 2 success rates reported in the high-90s and Tier 3 targets dropping to roughly 70–85%. One directory scores it 3.9/5 with a 7.8/10 trust score, and cites a 97% success rate and around 1,300 ms average response — slower than Shifter's vendor-reported figure, by a margin you should expect at this price.

One thing worth flagging: nearly everything ranking for a 9Proxy review is written by a company that sells proxies, including at least one competitor page that questions the vendor's corporate details. Keep that in mind for both brands, not just this one.

If the per-gigabyte difference is the part that matters for your workload, 👉 [check 9Proxy's current residential pricing and plans here](https://bit.ly/9-Proxy) before you commit to a 200 GB package elsewhere.

## Shifter vs 9Proxy, side by side

|  | Shifter | 9Proxy |
| --- | --- | --- |
| Residential pool (advertised) | 205M+ IPs, 195+ countries | 20M+ IPs, 90+ countries |
| Entry rate | $2.00/GB (5 GB, $10) | $3.00/GB (5 GB, $15) |
| Best published rate | $0.75/GB from 200 GB | $0.68/GB at 10,000 GB |
| 100 GB cost | $100 | $150 |
| Billing models | Per GB only | Per GB or per IP with unlimited bandwidth |
| Targeting | Country, city, ASN | Country, state, city, ZIP, ISP |
| Unlimited-bandwidth option | No (legacy port plans only) | Yes, on IP plans |
| Validity | Not stated per tier | 180 days, unlimited on Enterprise |
| Free trial | None; ~72-hour money-back | Limited trials vary by availability |
| Protocols | HTTP(S), SOCKS5 | HTTP(S), SOCKS5 |
| Third-party rating | 3.8/5 (directory), 4.8/5 (another) | 3.9/5 (directory) |
| Reported success rate | 98.43% (directory) | 97% (directory) |

The pattern in that table is simple: Shifter is cheaper per gigabyte at mid volumes, 9Proxy is cheaper at the very top end and much cheaper if your workload suits unlimited-bandwidth IP plans instead of traffic billing.

## Which one to buy

**If you're scraping 200 GB a month or more and your costs scale with page weight,** Shifter's $0.75/GB is hard to beat on the published cards, and the city/ASN targeting included at every tier is the reason its benchmark pages exist. Budget for the fact that you'll be testing inside a 72-hour window.

**If your traffic per request is tiny but your rotation needs are high** — ad verification, geo checks, API polling, price sampling across many cities — per-gigabyte billing works in your favour, so the choice comes down to which provider holds up on your specific targets rather than which rate card looks smaller.

**If you run long sessions with heavy data transfer on the same IP,** the unlimited-bandwidth IP model is the structural answer, and Shifter doesn't sell that anymore. That's 9Proxy's territory, at $0.24/IP at the smallest tier and down to roughly $0.02/IP at scale. Start at 100 IPs, not 100,000.

**If you need mobile or datacenter proxies too,** neither of these is a complete answer — 9Proxy's documented product lines are residential only, and Shifter's datacenter options appear mostly in the older backconnect framing.

👉 [Compare 9Proxy's IP-based and GB-based packages side by side](https://bit.ly/9-Proxy)

## Straight answers to the usual questions

**Is Shifter legit, or a scam?** It has operated since 2012 under three names, its rebrand from MicroLeaves is documented on its own site, and it publishes a full rate card without gating prices behind sales calls. The real complaints in user reviews are about support responsiveness and connection errors, plus a short 72-hour refund window and no free trial. Those are service-quality problems, not fraud signals.

**Can you still buy port-based unmetered plans?** Some comparison tables still list them, at figures like $299.99 for 25 ports. The vendor's own position is that bandwidth pricing has replaced them and that legacy customers can have their old usage mapped onto an equivalent traffic plan. If a page is selling you ports, check the date on it.

**Is 9Proxy cheaper than Shifter?** At entry level, yes — $3.00/GB versus $2.00/GB is the one place Shifter wins, and from 100 GB upward Shifter is ahead until you reach the 10,000 GB Enterprise tier. But if your workload fits the unlimited-bandwidth IP model, the comparison stops being about per-GB rates entirely: 100 IPs at $0.24 each with unlimited traffic is a different unit of measurement, and usually a much smaller invoice.

**Do both support sticky sessions?** Yes. Shifter supports sticky sessions on its gateway, and 9Proxy offers a sticky mode where the IP changes when the configured session time ends, alongside a rotating mode that switches per request.

**What should you test first?** Whichever provider you pick, run your own request batch against your hardest target before buying a large package. The vendor benchmarks published by both sides use their own methodology, the directory numbers use a different one, and the gap between 364 ms and 1,300 ms in the tables above is largely a gap between two measurement setups, not a settled fact about either network.

👉 [Start with a small 9Proxy package and test it on your own targets](https://bit.ly/9-Proxy)

## Bottom line

Shifter is a 2012-era provider that rebranded into a cleaner, publicly priced product, and its $0.75/GB mid-volume rate is genuinely competitive. What holds it back isn't the price card — it's the lack of a free trial, a refund window measured in hours, a legacy MicroLeaves site that still confuses search results, and speed claims that only exist on its own domain.

9Proxy is the smaller, cheaper, residential-only option. Its 90+ country footprint is roughly half of what Shifter advertises, its directory-reported latency is slower, and its city targeting has been questioned by at least one competitor. But it sells the thing Shifter no longer does — unlimited bandwidth per IP — and its per-gigabyte rate at high volume undercuts Shifter's best published number.

Pick on structure, not brand: per-gigabyte billing for scrape-heavy loads with predictable page sizes, per-IP unlimited bandwidth for long sessions and unpredictable transfer. And whichever way you go, spend your first week measuring your own success rate, because the published evidence for both providers is thinner than their rate cards suggest.

👉 [See 9Proxy's live residential proxy packages and current rates](https://bit.ly/9-Proxy)
