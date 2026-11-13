# Switzerland VPS: What 1 GB Really Costs, Which Tier You Actually Need, and How to Test a Zurich Box Before You Pay

A 1 GB VPS in a Swiss datacentre lists at CHF 6 (iFog, Zurich), €4.99 (EDIS Global, Interxion Glattbrugg) and €8 (Colonelserver). Three prices, three currencies, same nominal RAM, and the spec sheets barely explain the gap. What you are buying at those numbers is the address: a rack near Zurich Airport, a 10 Gbps uplink instead of 1 Gbps, an IPv6 block instead of a single address, and hardware sitting under Swiss jurisdiction.

Below: what a Swiss VPS should cost, where JustHost's current VPS catalogue sits against that benchmark, the contract clauses that change the real annual bill, and the ten-minute test to run before you pay anyone.

> **Quick pick.** 2 GB is the sensible floor for anything with a database. JustHost's Arcturus gives 1 core, 2 GB RAM, 30 GB NVMe and a 300 Mbps fair-share port for **$3.21/month on a 12-month prepay** ($4.01 month-to-month). A static site, a DNS node or one WireGuard endpoint runs fine on 1 GB (Sirius, **$2.25/month** prepaid annually). 👉 [Check JustHost's current VPS prices](https://justhost.asia/en/vps?ref=196392)

## JustHost's VPS line-up and what each tier costs

JustHost runs one VPS catalogue across a network its homepage counts at 80 data centres in 41 countries. The plan pages don't name locations, so the order form's location picker is where you confirm Switzerland is selectable for the plan you want. Check that before paying, not after.

Prices below are monthly equivalents. The first figure assumes a 12-month prepay, which is where the site's displayed 20% discount applies; the second is the month-to-month rate. USD figures come from the English VPS page; plans that only carry a ¥ price appear on the fuller Chinese-locale tariff list.

| Plan | vCPU / RAM | NVMe | Port (fair-share, unmetered) | Price (12-mo / monthly) | Order |
| --- | --- | --- | --- | --- | --- |
| Sirius | 1 core / 1 GB | 20 GB | 300 Mbps | $2.25 / $2.81 | [ Order Sirius](https://justhost.asia/services/vps/tariffs/sirius?ref=196392) |
| Arcturus | 1 core / 2 GB | 30 GB | 300 Mbps | $3.21 / $4.01 | [ Order Arcturus](https://justhost.asia/services/vps/tariffs/arcturus?ref=196392) |
| Alpha Centauri | 2 cores / 2 GB | 40 GB | 400 Mbps | ¥48.37 / ¥60.46 | [ Order Alpha Centauri](https://justhost.asia/services/vps/tariffs/alpha_centauri?ref=196392) |
| Vega | 2 cores / 4 GB | 80 GB | 500 Mbps | $6.23 / $7.79 | [ Order Vega](https://justhost.asia/services/vps/tariffs/vega?ref=196392) |
| Capella | 4 cores / 4 GB | 120 GB | 750 Mbps | ¥98.46 / ¥123.08 | [ Order Capella](https://justhost.asia/services/vps/tariffs/capella?ref=196392) |
| Rigel | 4 cores / 8 GB | 200 GB | 750 Mbps | ¥150.28 / ¥187.86 | [ Order Rigel](https://justhost.asia/services/vps/tariffs/rigel?ref=196392) |
| Antares | 5 cores / 8 GB | 300 GB | 750 Mbps | ¥178.12 / ¥222.65 | [ Order Antares](https://justhost.asia/services/vps/tariffs/antares?ref=196392) |
| Betelgeuse | 6 cores / 12 GB | 400 GB | 750 Mbps | $21.12 / $26.40 | [ Order Betelgeuse](https://justhost.asia/services/vps/tariffs/betelgeuse?ref=196392) |
| Spica | 8 cores / 16 GB | 500 GB | 750 Mbps | ¥328.41 / ¥410.51 | [ Order Spica](https://justhost.asia/services/vps/tariffs/spica?ref=196392) |
| Altair | 8 cores / 24 GB | 600 GB | 750 Mbps | $37.92 / $47.40 | [ Order Altair](https://justhost.asia/services/vps/tariffs/altair?ref=196392) |
| Aldebaran | 8 cores / 32 GB | 700 GB | 750 Mbps | ¥662.38 / ¥827.98 | [ Order Aldebaran](https://justhost.asia/services/vps/tariffs/aldebaran?ref=196392) |
| Procyon | 12 cores / 32 GB | 1,000 GB | 1,000 Mbps | ¥885.04 / ¥1,106.30 | [ Order Procyon](https://justhost.asia/services/vps/tariffs/procyon?ref=196392) |

There is a second, cheaper line where you pick the storage type yourself. Same core counts, smaller disks, and this is where the real entry price sits:

| Constructor tier | HDD | SSD | NVMe |
| --- | --- | --- | --- |
| Start, 1 core / 512 MB / 5 GB | $2.60 | $3.12 | $3.38 |
| Standard, 2 cores / 2 GB / 25 GB | $8.80 | $10.56 | $11.44 |
| Super, 4 cores / 4 GB / 50 GB | $17.60 | $21.12 | $22.88 |

IPv6-only instances start at $1.60/month; the cheapest dual-stack configuration is $2.60/month. All prices in both tables are the 12-month-prepay monthly equivalents.

One thing to know about the "unmetered" label before you compare it to a Swiss plan with a traffic quota. JustHost's own arithmetic converts the 300 Mbps fair-share port to "93+ TB monthly". That is a port speed, not a traffic allowance, and the site sells bandwidth as a paid extra: +10 Mbps at ¥16.80/month, an extra IPv4 at ¥22.29/month, and a dedicated 1 Gbps uplink at ¥2,240.85/month.

Reviews of the brand are mixed. Trustpilot entries from early 2026 describe an outage on 2 March 2026 with no status updates for roughly 15 hours, and several complain that first-line support is a bot. Budget for the possibility that you are your own sysadmin. 👉 [See the full JustHost VPS list and pick a tier](https://justhost.asia/en/vps?ref=196392)

## What a Swiss VPS should cost

Expect CHF 4 to €8 for 512 MB to 1 GB inside a Swiss datacentre, and CHF 10 to €17 for 4 GB. Here is what providers with a Swiss presence publish today.

| Provider | Swiss location | Cheapest tier listed | What's included at that price | Fine print |
| --- | --- | --- | --- | --- |
| iFog | Zurich | CHF 4/mo for 512 MB; CHF 6/mo for 1 GB | 1 shared Xeon core, 25 GB SSD, 4 TB on 1 Gbit/s, 1 IPv4 + IPv6, daily backup | Linux templates only; manual activation up to 24 h; optional BGP session |
| EDIS Global | Zurich, Interxion Glattbrugg | €4.99/mo excl. VAT for 1 GB | 1 AMD EPYC vCPU, 15 GB NVMe, 1 TB traffic, 2×10 Gbps uplink | Annual prepay includes one month free; Windows needs a higher tier |
| Colonelserver | Switzerland | €8/mo for 1 GB | 1 core, 40 GB, unlimited traffic on a 1 Gbps port, DDoS protection | Fully unmanaged Linux; the page calls the disk NVMe in the headline and "SSD Storage" in the table |
| SwissLayer | Switzerland | $19.95/mo, but that's the 2 GB plan | 2 Xeon E5-2670 cores, 30 GB SSD, 5 TB, 1 IPv4 + 100 IPv6 | No 1 GB tier on the page reviewed |
| OVHcloud | Zurich and Geneva local zones | Not published on the page reviewed | Xeon vCPU, NVMe, KVM, vRack private networking, DDoS protection, unlimited traffic | Several plan families (SSD, Cloud, unmanaged, backup, reseller) sold separately |

Six things explain the spread, and none of them is core count:

1. **Virtualisation and CPU class.** iFog sells shared Xeon cores; EDIS sells AMD EPYC vCPUs. A "1 core" label means different things.
2. **Disk type.** NVMe versus SSD shows up in database latency long before it shows up in your invoice.
3. **Uplink.** EDIS advertises 2×10 Gbps. iFog and Colonelserver run 1 Gbps ports. A shared 10 Gbps uplink is not 10 Gbps to your VM, but it does reduce contention at peak.
4. **IPv6 allocation.** One address at iFog (with prefixes up to /48 as an add-on), 100 addresses at SwissLayer. If you run proxies or per-customer isolation, this is a real line item.
5. **Backups.** Included daily at iFog, an optional add-on at SwissLayer.
6. **Tax and provisioning.** EDIS states prices Excl. VAT; iFog and Colonelserver don't say either way. iFog provisions manually, up to 24 hours.

## What the sticker price leaves out

1. **VAT is not always in the number.** EDIS marks every plan "Excl. VAT". On a €4.99 plan the amount that leaves your account at checkout is higher, and how much depends on your billing country.
2. **The discount lives in the annual prepay.** EDIS gives 12 months for the price of 11. JustHost's headline prices assume a 12-month term: Sirius drops from $2.81 to $2.25, Vega from $7.79 to $6.23, roughly 20% in each case. Month-to-month costs more, and that's the number to compare if you might leave in three months.
3. **Resizing usually means downtime.** EDIS states plainly that RAM, vCPU and storage changes require a full shutdown and restart, and that after a storage upgrade you resize the partition and filesystem yourself.
4. **Changing datacentre has a deadline.** At EDIS you can move a VPS to another location only within 24 hours of activation. If you are unsure whether Zurich or Frankfurt is right, decide fast or buy a second small box to test.
5. **Windows needs a bigger plan.** EDIS says KVM Smart (1 GB) and KVM Starter (2 GB) are not suitable for Windows Server and points to KVM Basic Plus or above. iFog doesn't sell Windows at all. JustHost's plan pages don't state Windows licensing terms, so ask before ordering if RDP is the plan.
6. **"Unlimited" is a port, not a counter.** Colonelserver writes unlimited traffic on a 1 Gbps port; iFog writes "8 TB on 1 Gbit/s" for its 2 GB plan; EDIS writes 1–4 TB quotas on a 2×10 Gbps uplink. Traffic allowance and port speed limit you in different ways, and a host can be strict on one while generous on the other.
7. **Instant versus manual delivery.** iFog activates every VPS by hand, up to 24 hours. If you need a box in five minutes, that matters more than CHF 2.

## How to check whether a Zurich box is actually fast

Published gigabit figures are almost always a host machine talking to one nearby speedtest server, not your VPS talking to your users.

EDIS, for example, publishes Speedtest CLI results from a host named kvm-lps-ch-zrh03, taken 21 September 2026: 9,306.85 Mbps down, 2,492.54 Mbps up and 1.03 ms idle latency to Sunrise in Zurich, and 9,328.15 / 2,463.67 Mbps at 0.57 ms to GGA Maur in Ebmatingen, both with zero packet loss. The same page states that the result is not a guarantee of individual VPS throughput or latency to other destinations. Read it that way: the Zurich network fabric is fast and the carriers are close, and your 1 GB slice will not see 9 Gbps.

The useful test is the boring one. Before ordering, find the provider's Looking Glass or test IP and run ping, traceroute and MTR from the network your users are on, over IPv4 and IPv6. Look at the route, not just the latency number: a Zurich box that tromboned through Frankfurt and back will beat a Frankfurt box on paper and lose in practice. Several hosts also publish 100 MB and 1 GB test downloads, which measure throughput to your connection rather than to a speedtest server inside the same building.

After that, check where your users actually sit. Zurich and Geneva are not the same distance from Milan, Munich and Lyon, and OVHcloud's pitch for its two Swiss local zones is specifically that in-country hosting beats "relying only on Frankfurt" for Swiss end users. That claim is easy to test with a traceroute and hard to test from a marketing page.

## Which tier for which job

- **Static site, redirector, DNS node, one WireGuard endpoint:** 512 MB to 1 GB. JustHost's HDD Start at $2.60 or Sirius at $2.25; iFog's CHF 4 box if you want a Swiss address with a daily backup included.
- **Single WordPress site with a cache in front, small API, monitoring host:** 2 GB. Arcturus at $3.21, EDIS KVM Starter at €8.49, Colonelserver at €12.
- **WooCommerce, multi-tenant API, anything with a search index:** 4 GB and NVMe. Vega at $6.23 on JustHost. At EDIS the 4 GB tier has two published versions on the same page: €10.49 for 1 vCPU in the plan card, €14.69 for 2 vCPU in the comparison table at the bottom. Ask which one applies to the configuration you're buying. Colonelserver lists 4 GB with 60 GB for €17.
- **Windows or RDP:** 4 GB minimum, and confirm the plan is Windows-eligible in writing before paying.
- **Staging, CI runners, throwaway test boxes:** the cheapest tier plus a backup add-on. 👉 [Open the Vega plan page for the 4 GB configuration](https://justhost.asia/services/vps/tariffs/vega?ref=196392)

## Does hosting in Switzerland do anything for compliance?

Only as much as the contract says, and the marketing pages reviewed here don't go further than assertions. OVHcloud states that data stays in Switzerland, aligning with national privacy rules and GDPR, aimed at finance, healthcare and government. EDIS, Colonelserver and SwissLayer all sell privacy-oriented infrastructure as a headline benefit.

None of these pages published a third-party certification or audit report to back the claim. Treat it as a vendor description and ask for the paperwork that actually binds them: a data processing agreement, the list of sub-processors, where backups are stored, and whether support staff access systems from outside Switzerland. The datacentre address is verifiable (Interxion's facility at Sägereistrasse 35 in Glattbrugg, for instance); "Swiss data protection" as a slogan is not.

## FAQ

### Do I need a Swiss datacentre at all?

If your users are in Switzerland, southern Germany, Austria or northern Italy, a Zurich box saves real milliseconds over Frankfurt, and the local hosts price that at CHF 4 to €8 for the smallest tier. If your users are spread across three continents, the location matters less than the route quality, and a cheap box elsewhere with a good backbone will do.

### Does local hosting help rankings on a .ch domain?

OVHcloud states that local hosting improves SEO signals for .ch domains. No search engine documents server location as a ranking factor, so treat it as a hosting vendor's claim. Page speed, hreflang and content do the work that location is credited with.

### What can a 512 MB or 1 GB box actually run?

512 MB handles a DNS resolver, a WireGuard endpoint, a static site behind nginx, or a small bot. 1 GB handles a single-site WordPress with caching, a small API, or a monitoring node. Add a database plus WooCommerce plugins and 2 GB is the floor, 4 GB the comfortable pick.

### Are these prices with or without tax?

It depends on the seller. EDIS marks prices Excl. VAT; iFog and Colonelserver don't state it on the pages reviewed; JustHost's listed prices don't say. The only reliable check is the checkout total before you confirm, which is also where a 12-month term gets applied.

### Can I start monthly and upgrade later?

Yes, with caveats. JustHost prices month-to-month at the higher rate in the table above, so you pay roughly 20% more for the flexibility. EDIS allows upgrades up to 8 vCPU, 24 GB RAM and 500 GB total storage, but RAM, vCPU and disk changes need a full shutdown, and extra IPv4 addresses cost €5/month each up to ten.

## Before you pay

Match the tier to the job and stop optimising past that point. A static site or a single tunnel needs 512 MB to 1 GB, nothing more. A site with a database needs 2 GB. Anything serving concurrent checkout traffic, or a Windows desktop, needs 4 GB and NVMe, and deserves a second look at whether the host's support can answer a ticket at 2 a.m.

Then confirm two things at checkout: whether the total includes tax and what term you just agreed to, and whether Switzerland appears in the location list for that specific plan. Once those are settled, run a traceroute from your own network to the host's published test IP before committing to a year.

👉 [Pick a JustHost plan and confirm the Swiss location at checkout](https://justhost.asia/?ref=196392)
