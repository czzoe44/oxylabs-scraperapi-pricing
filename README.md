# oxylabs pricing: Real Costs and Hidden Minimums Explained — Plus When a Credit-Based ScraperAPI Plan Costs Less

Oxylabs pricing starts at **$30/month** on the Starter plan, which buys residential traffic at **$6/GB** (about 5 GB). The full ladder runs Starter $30 → Basic $100 → Flexible $500 → Enterprise from $2,500/month, and as of October 2026 one subscription now covers every Oxylabs product — residential, mobile, ISP, datacenter proxies, the Web Scraper API, Web Unblocker, and its AI headless browser. That last part is the headline change, but the number that actually decides your bill is a different one: whether you pay per GB or per result. On heavy, JavaScript-rendered pages, that single difference can swing your effective cost per 1,000 pages by a factor of eighteen.

If your use case is API-based scraping rather than raw proxy bandwidth, this article also covers ScraperAPI, a credit-billed alternative whose plans start at $49/month with rendering, premium residential IPs, and CAPTCHA handling included — no per-parameter surcharges for the basics. We'll walk through both pricing systems with real per-page math so you can see which one fits your target sites.

> **Quick take:** Most people searching Oxylabs pricing want a cost-per-page answer, and the answer depends on page weight. If your targets are e-commerce or general websites and you'd rather pay per successful request than per GB, ScraperAPI's Hobby plan at $49/month (100,000 credits, annual billing drops it to $44.10) is the lower-commitment entry point, and a 7-day trial with 5,000 credits lets you verify costs before paying. 👉 [View ScraperAPI's plans and start the free trial](https://www.scraperapi.com/pricing/?fp_ref=coupons)

## Oxylabs Pricing Plans: The Current Lineup

As of October 2026, Oxylabs sells a single subscription ladder that sets your rate on every product at once. Before the consolidation (visible in captures as recent as September 2026), each product had its own plan tiers; now you pick one level and every meter prices off it.

| Plan | Monthly Fee | Residential Rate | Notes |
| --- | --- | --- | --- |
| Starter | $30 | $6/GB | ~5 GB of residential traffic |
| Basic | $100 | $5/GB | ~20 GB residential |
| Flexible | $500 | $4/GB | Marked "Most popular" |
| Enterprise | From $2,500 | $2.50/GB | Sales quote; rates negotiable |

The same tier logic drives other products: mobile starts at $7.50/GB (dropping to $3.50/GB at the top tier), ISP proxies from $1.50/IP, dedicated datacenter from $2/IP, and shared datacenter from $0.60/GB on bandwidth billing. Two API products bill differently — the /Search API is a flat $1 per 1,000 searches on every tier, and /Scrape (formerly the Web Scraper API) runs from $0.50 per 1K successful results down to $0.25 at higher tiers, with failed requests not billed.

New accounts get **$5 in free welcome credits** toward any product, and activating the free plan requires no payment information — you register, create a proxy user in the dashboard, and you're running.

One caution before you budget: there's no true pay-as-you-go on residential or mobile. Top-ups extend a plan rather than replace it, so your real monthly floor is $30 even if you only push 500 MB. Enterprise-tier prices are quoted by sales, and the published numbers are a floor, not a ceiling — at scale you negotiate.

## What a GB Actually Buys: Per-Page Cost Math

This is the part most Oxylabs pricing breakdowns skip, and it's where overpaying happens.

Bandwidth billing means your cost per page depends entirely on page weight. Working from the published rates:

| Product and tier | Rate | Per 1,000 pages at 250 KB | Per 1,000 pages at 1 MB |
| --- | --- | --- | --- |
| Datacenter shared, per GB | $0.59/GB | ~$0.14 | ~$0.58 |
| Residential Starter | $6/GB | ~$1.47 | ~$5.86 |
| Residential Enterprise | $2.50/GB | ~$0.61 | ~$2.44 |
| Mobile Starter | $7.50/GB | ~$1.83 | ~$7.32 |
| Web Unblocker entry | $9.40/GB | ~$2.30 | ~$9.18 |

Every per-GB line quadruples when your pages get heavy. Rendered, JavaScript-heavy pages routinely hit 1 MB or more, so a plan that looked cheap on lightweight HTML can cost four times your estimate in practice.

Success-billed products don't have this problem. Oxylabs' own Scraper API bills per delivered result — the entry tier works out to a flat $0.50 per 1,000 pages regardless of whether those pages weigh 250 KB or 2 MB. On 1 MB pages, the entry Web Unblocker tier costs roughly **eighteen times** what the Scraper API charges for the same page. The webscraping.cc analysis puts it plainly: checking the Scraper API price before buying Web Unblocker is "the single highest-value five minutes in this whole guide." If your target site is supported by their parser list, per-result billing usually wins.

## ScraperAPI Pricing: Full Plan Table

ScraperAPI takes the per-result idea further: you pay in API credits, one credit being a standard page request. Every paid plan includes JS rendering, premium residential and mobile IPs, CAPTCHA and anti-bot bypass, JSON auto-parsing, and unlimited bandwidth — those features aren't gated behind higher tiers. Annual billing takes **10% off** every plan, and there's a **7-day free trial with 5,000 credits, no credit card required**.

| Plan | Monthly | Annual (per mo.) | Credits | Concurrency | Geotargeting |
| --- | --- | --- | --- | --- | --- |
| Free | $0 | — | 1,000 | 5 | — |
| Hobby | $49 | $44.10 | 100,000 | 20 | US & EU |
| Startup | $149 | $134.10 | 1,000,000 | 50 | US & EU |
| Business | $299 | $269.10 | 3,000,000 | 100 | Country-level |
| Scaling | $475 | $427.50 | 5,000,000 | 200 | Country-level |
| Professional | $975 | $877.50 | 10,500,000 | 300 | Country-level |
| Advanced | $1,975 | $1,777.50 | 21,500,000 | 500 | Country-level |
| Enterprise | Custom | Custom | 22M+ | 500+ | Country-level |
| Plan | Get Started |  |  |  |  |
| --- | --- |  |  |  |  |
| Hobby | [Get Hobby at the annual rate](https://www.scraperapi.com/pricing/?fp_ref=coupons) |  |  |  |  |
| Startup | [Get Startup at the annual rate](https://www.scraperapi.com/pricing/?fp_ref=coupons) |  |  |  |  |
| Business | [Get Business at the annual rate](https://www.scraperapi.com/pricing/?fp_ref=coupons) |  |  |  |  |
| Scaling | [Get Scaling at the annual rate](https://www.scraperapi.com/pricing/?fp_ref=coupons) |  |  |  |  |
| Professional | [Get Professional at the annual rate](https://www.scraperapi.com/pricing/?fp_ref=coupons) |  |  |  |  |
| Advanced | [Get Advanced at the annual rate](https://www.scraperapi.com/pricing/?fp_ref=coupons) |  |  |  |  |

The per-credit price drops sharply early — Hobby to Startup cuts unit cost by about 70% — then flattens. From Business upward, the rate sits between $0.092 and $0.100 per 1,000 credits across a six-fold jump in price, so beyond Business you're buying concurrency and volume rather than a better rate.

Two limits worth knowing before you pick a cheap tier: Hobby and Startup only support **US and EU** geotargeting, so if you need to appear as a user in a specific country, you need Business or above. And on Analytics, the two lower tiers only keep the last 30 days of data.

## How ScraperAPI Credits Are Charged

A standard page costs 1 credit, but costs scale with domain complexity and the options you enable. The official rates:

| Request Type | Credits per Request |
| --- | --- |
| Standard page | 1 |
| Amazon, Walmart, eBay | 5 |
| Google, Bing (all subdomains) | 25 |
| LinkedIn | 30 |
| `render=true` (JS rendering) | +10 |
| `premium=true` (premium residential/mobile IP) | +10 |
| `premium=true` + `render=true` | 25 |
| `ultra_premium=true` + `render=true` | 75 |
| Cloudflare / Datadome / PerimeterX / Akamai bypass | +10 |

Note what *doesn't* cost extra: `country_code`, `autoparse`, session control, device type, output format. Setting a country target or auto-parsing the response is free, which matters when comparing against providers that meter every option.

The useful part is predictability. Before running anything at scale, you can look up any URL's exact credit cost in the dashboard's Domain Multiplier, test it in the API Playground, or call a cost-check API endpoint that accepts all parameters. Each response also carries a `sa-credit-cost` header showing what that request consumed, and you can set a `max_cost` cap per scrape so a single job can't blow past your limit. Oxylabs offers no equivalent per-page cost forecaster — you estimate bandwidth and find out from the meter.

Billing is success-based: only 200 and 404 responses are charged, plus requests you cancel yourself before the 70-second completion window closes. If you exceed your plan's concurrency limit, you get a 429 and the request is turned away — there's no overage charge. When credits run out, scraping pauses by default, but Hobby through Professional can opt into auto-upgrade (moving to the next plan automatically), and Scaling and above can keep scraping on pay-as-you-go at a fixed per-credit rate under a monthly cap you set.

👉 [Sign up for the free 1,000-credit plan](https://www.scraperapi.com/signup?fp_ref=coupons) and run your actual target URLs through the cost estimator before deciding on a tier — the numbers you get back are the real budget, not an estimate.

## Oxylabs vs. ScraperAPI: Which Pricing Model Fits Your Project

Both are legitimate, well-established providers — Oxylabs runs a 175M+ residential IP pool across 195 locations with ISO 27001 and SOC 2 certifications on its main API lines, while ScraperAPI is a smaller, API-first operation. The choice is mostly about billing model and workflow.

**Oxylabs fits better when:**

- You need raw proxy infrastructure — residential, mobile, ISP, and datacenter pools — and already have your own scraping stack
- You need long-lived sessions on a single identity (ISP proxies from $1.60/IP/month) or unlimited-concurrency residential bandwidth
- You're scraping simple, lightweight pages at high volume, where shared datacenter bandwidth at ~$0.14 per 1,000 pages is hard to beat
- You want per-result billing on supported targets through their Scraper API at $0.50/1K

**ScraperAPI fits better when:**

- Your targets are Amazon, Google SERPs, or general websites and you want one API call to handle rendering, proxies, retries, and CAPTCHAs
- Page weight varies or skews heavy — per-credit billing is immune to it, per-GB isn't
- You're a solo developer or small team; a $49 Hobby plan with 100K credits is a much smaller commitment than any bandwidth plan with a $30 floor and usage-based surprises
- You want to know exactly what a scrape will cost before running it

A concrete comparison on Google searches: each SERP request costs 25 credits on ScraperAPI, so the Business plan's 3M credits covers 120,000 searches for $299 — about $2.49 per 1,000. Oxylabs' /Search API charges a flat $1 per 1,000 searches on any tier, so at high sustained SERP volume, Oxylabs is cheaper. At moderate volume, ScraperAPI's included parsing, retries, and bypass work close the gap — and you're not managing proxy infrastructure.

One structural difference to keep in mind: Oxylabs' residential and mobile tiers carry unlimited concurrent sessions, so for many parallel tasks, residential bandwidth can be the better deal even when ISP looks cheaper per unit. But watch the concurrency cliffs on the IP-billed products — dedicated datacenter proxies allow 100 concurrent sessions per IP until you cross 100 GB in a month, after which it drops to 10 per IP until your billing cycle resets. The same throttling applies to ISP proxies at a 50 GB threshold. Getting your throughput back means buying ten times the IPs, which turns a $16 ISP plan into $160.

## First-Year Cost Scenarios

Monthly prices hide the compounding. Here are two realistic setups.

**Mid-size residential scraping, ScraperAPI Business, annual:** $269.10 × 12 = **$3,229.20** for year one, renewing at the same rate, with ~3M credits/month — enough for roughly 600,000 Amazon pages or 120,000 Google searches per month before any parameter overhead.

**Same volume on Oxylabs residential:** 600,000 Amazon-style product pages at ~500 KB each is ~300 GB/month. On the Flexible tier at $4/GB, that's $1,200/month for bandwidth alone — plus rendering and retry overhead you'll absorb as extra traffic. Bandwidth billing punishes exactly the sites that are hardest to scrape.

Flip it for lightweight work: a static-site crawl at 250 KB per page on shared datacenter bandwidth costs ~$0.14 per 1,000 pages, and no credit-based API matches that. Bandwidth pricing wins when pages are light and you bring your own logic.

## FAQ

**Does Oxylabs have a free trial?**
Yes, but it varies by product. The Scraper API and Web Unblocker offer self-serve trials with no card required, and every new account gets $5 in welcome credits. Residential, mobile, and ISP proxy trials go through their support team or a scheduled demo, and each customer gets one trial — so don't waste it on a test URL you don't care about.

**Does ScraperAPI have a free plan?**
Yes — 1,000 free credits with up to 5 concurrent connections, no card needed. Support can grant extra testing credits if you ask. The 7-day trial with 5,000 credits sits on top of that for evaluating paid features.

**Is there a discount on either service?**
ScraperAPI applies 10% off automatically on annual billing for every plan — no code to enter. Oxylabs has run promotional pricing on specific products (a 40% discount on Web Unblocker was active during recent checks), but those promos expire after six months, so build your budget on list prices.

**What happens when I hit my limits?**
On Oxylabs, residential and mobile top-ups extend your plan, and the IP-billed products throttle concurrency once you cross their monthly GB thresholds. On ScraperAPI, over-limit requests return a 429 with no charge, credits running out pauses scraping until renewal (or triggers opt-in auto-upgrade), and Scaling-tier plans and above can keep going on pay-as-you-go under a self-set cap.

## Which Should You Pick?

Confirm two things before subscribing to either service: your realistic monthly page volume with actual page weights (a week of real traffic through a trial settles it), and whether you need country-level geotargeting — on ScraperAPI that single requirement moves you from Startup to Business.

If you have your own scraping stack, need dedicated IP pools, or your pages are small and static, Oxylabs' bandwidth pricing — from $30/month — will be cheaper, and its Enterprise tier negotiates well at scale. If you want rendering, CAPTCHA handling, and parsed output bundled into one API call, or you simply can't tolerate bandwidth-meter surprises on heavy pages, ScraperAPI's credit model is the safer budget: start free, check your target URLs' real costs, and only pick a tier once the numbers are yours. 👉 [Compare ScraperAPI's plans and start the 7-day free trial](https://www.scraperapi.com/pricing/?fp_ref=coupons) — 5,000 credits, no card required.
