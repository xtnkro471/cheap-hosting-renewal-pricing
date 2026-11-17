# Cheap Web Hosting: Is Under $10 a Month Real, What Happens at Renewal, and When Does a $10-a-Year VPS Make More Sense? (Full Plan and Price Table)

Cheap web hosting has a working definition: a **regular annual price of $10 per month or less**, which is the cutoff PCMag uses for its cheap hosting roundup. Introductory discounts don't count toward that number, because a host that charges $6 for twelve months and $10 after that isn't a $6 host. Two live examples show the size of the gap. IONOS advertises **$6/month on a one-year term, then $10/month**. OVHcloud's Agency Max runs **$29.49/month for the first 12 months ($353.88 total) and renews at $90.89/month**, which is $1,090.68 a year.

That gap is what this article is about. It covers what a realistic cheap plan includes, where RackNerd's shared and VPS products sit against the market, which limits only show up in the terms of service, and how to decide between a $9/month shared plan and an annual VPS that costs less per year than two months of shared hosting.

## Quick pick: what most readers should buy

> **Want a control panel and no server administration:** RackNerd's shared hosting, listed at **$9.59/month** for 100 GB SSD, 3 TB monthly transfer, no cap on websites or databases, free SSL and daily backups. It clears the $10 line, just barely.
>
> **Comfortable on the command line:** the KVM VPS specials are where the low prices actually live. These are unmanaged boxes with full root SSH access, a 1 Gbps port and a control panel for reboots, OS reinstalls and one-click apps. Entry configurations have sold for as little as about $11/year, with 2 GB plans around $36/year.
>
> 👉 [See RackNerd's current shared and VPS listings](https://bit.ly/RacKnerd)

## RackNerd plans and prices

RackNerd sells two things a cheap-hosting buyer will look at: shared hosting and promotional KVM VPS plans. The VPS side is priced per configuration and rotates with each promotion, so the number you pay depends on the box you pick on the order page.

| Plan | What you get | Price | Billing | Order |
| --- | --- | --- | --- | --- |
| Shared Hosting 100 GB | 100 GB SSD, 3 TB/month transfer, unlimited websites and databases, free SSL, daily backups (best effort) | **$9.59/mo** | Monthly | [Check the shared plan](https://bit.ly/RacKnerd) |
| KVM VPS Specials | Unmanaged KVM VPS, full root SSH, 1 Gbps port, ctrl panel with reboot, OS reinstall, HTML5 VNC console, network firewall and one-click apps; CentOS, Rocky, AlmaLinux, Fedora, Debian or Ubuntu | Promo pricing per configuration; annual specials have run from about **$11/yr** | Annual (promotional) | [See current VPS specials](https://bit.ly/RacKnerd) |

Two things about that table matter more than the numbers. First, the VPS line is **unmanaged by default**: RackNerd supplies hardware, network, power and infrastructure support, and you handle the OS, security, firewall, software updates, backups and troubleshooting. Server management is available as a paid extra. Second, the shared plan is a normal monthly bill at roughly the market rate for a mid-tier shared account, not a loss-leader. If your budget is genuinely a few dollars a month, the VPS specials are the only part of the catalog that gets you there.

The VPS hardware is KVM with full root access, and the ctrl panel covers the day-to-day work: power control, OS reinstalls, an out-of-band HTML5 console for recovery, inbound firewall rules, root password resets and upgrades. One-click apps include Docker with Portainer, n8n, Coolify, Ollama, LibreChat, AnythingLLM and several agent tools; the AI workloads want at least 4 GB of RAM, and OpenClaw wants 8 GB. Anything not in the catalog you install yourself over SSH, which is the point of root access.

## What cheap hosting costs elsewhere

These are advertised prices from each provider's own pages, using the billing term they quote. Treat them as a floor, not a final number.

| Provider | Plan | Advertised price | Billing basis |
| --- | --- | --- | --- |
| Namecheap | Stellar shared | $2.28/mo | Promotional |
| DigitalOcean | Droplets (VPS) | from $4/mo | Monthly |
| IONOS | Cheap hosting | $6/mo, then **$10/mo** | 1-year term |
| Hostwinds | Shared | $6.99/mo | Billed annually |
| Liquid Web | Digital storefront | $9/mo, $8.10/mo annual | Monthly or annual |
| HostArmada | Spark VPS | $9.88/mo, $8.20/mo annual | Monthly or annual |
| OVHcloud | Agency Max | $29.49/mo, renews at **$90.89/mo** | 12-month term |

RackNerd's shared plan at $9.59/month lands in the middle of that group, above Namecheap's promotional sticker and below OVHcloud's renewal cliff. Its VPS specials sit in a different category entirely: $11 to roughly $36 a year is below what most providers charge for a single month of a comparable self-managed server. The trade is that you're the system administrator.

DigitalOcean is the closest structural comparison on the VPS side at $4/month, and the difference is billing and support scope. DigitalOcean sells infrastructure with a 99.99% uptime SLA and expects you to build on it. RackNerd sells a promotional annual box with a 1 Gbps port and a control panel, and also expects you to build on it. Neither includes a site builder, and neither will design anything for you.

## The fine print that actually costs money

**There is no money-back guarantee.** RackNerd's terms, last revised in July 2026, state that refunds are not provided by default once payment is received, on the grounds that provisioning has real costs. Requests are handled case by case through a billing ticket, and a used service should be expected to get a no. Compare that with Namecheap, whose 30-day refund applies only to first-time shared and VPS customers who start without a trial, and excludes anyone opening a second account or re-registering after cancelling. Namecheap's dedicated servers get 7 days and exclude add-ons and licences. If a trial period is part of your decision, neither of these is the place to find one.

**Cancellation needs notice, not a click.** RackNerd requires written notice through the client area 5 days before the renewal date; contract services need 7 days and may carry an early-termination fee. Server data is removed immediately on cancellation, so pull your files first. Non-payment adds a 10% late fee after 3 days, and unpaid services are terminated 7 days after the due date with permanent data removal. Auto-renewal is the default state, which is how a $11 annual box quietly becomes a $11 annual box you forgot about.

**Backups are a courtesy, not a guarantee.** The shared plan includes daily JetBackup copies to Wasabi with up to 30 days of retention, and the terms describe this as best-effort, with availability, frequency, integrity and restorability all subject to variation. You're told to keep your own off-network backups. On an unmanaged VPS there's no host-side backup at all unless you buy one or script it.

**Shared hosting is for public websites only.** Cloud storage lockers, unrelated backup storage and video streaming are prohibited on the shared and reseller tiers, and RackNerd directs those uses to a VPS. Cryptocurrency mining, spam, brute-forcing, outbound DDoS and traffic exchange are prohibited everywhere, and nested virtualisation needs written approval. A chargeback on a service terminated for prohibited use carries a $125 to $250 administrative fee. Transferring a service to another client account costs $8.

**The uptime SLA pays out in credits, not refunds.** The guarantee is 99.9% monthly uptime for network transit and power, per service. Beyond that you get a 2% account credit of the monthly fee for each additional completed hour of downtime, capped at 50% a month, and you have to open a ticket within 30 days while the account is current. Scheduled maintenance is excluded for up to 180 minutes a month. Disputes go to arbitration under California law.

👉 [Read the current plans and terms before you pay](https://bit.ly/RacKnerd)

## Who should not buy this

**You want someone else to run the server.** Liquid Web's budget tier starts at $9/month ($8.10 annual) and includes full server maintenance, which is unusual at that price and is the reason it exists as a category. If "I don't want to touch SSH" describes you, an unmanaged $11/year VPS is the wrong purchase no matter how good the price looks.

**You need Windows or ASP.NET.** Linux hosting is cheaper and better suited to PHP workloads; ASP.NET and MSSQL need Windows hosting, which costs more across the board.

**You want a drag-and-drop site.** RackNerd gives you a server, not a website. DigitalOcean's own documentation makes the same point about its infrastructure products: you still need Squarespace or Wix or WordPress to build the actual site.

**You need 24/7 phone support at 3 a.m.** RackNerd advertises 24/7 support for platform issues, and the shared tier includes support, but an unmanaged VPS means the application layer is yours. Providers competing on managed hosting staff phone lines for exactly this reason.

## FAQ

**Can a $1 or $2 per month host actually work?**
For one small site with modest traffic, yes. Namecheap's Stellar plan at $2.28/month covers a blog or a portfolio, and IONOS's entry tier handles what its own FAQ calls "many applications and smaller projects." What the price doesn't include is headroom: GoDaddy's entry shared plan allows 1 website and 10 GB of NVMe storage, and IONOS's Essential tier is a single site. A second project means a second plan or an upgrade.

**Is annual billing worth it?**
On a $11 to $36 VPS, annual is the only way the price exists, so the real question is whether you'll still want the box in three months. Buy one year, not three, until you've lived with the service. On shared hosting, PCMag's advice is to avoid committing to an annual term before you know what features you need and how fast you expect to grow, because the renewal price is the one that sticks.

**Will my price double at renewal?**
It can more than double. OVHcloud's Agency Max goes from $29.49 to $90.89 a month. IONOS goes from $6 to $10. Before paying, find the renewal rate in the cart or the terms, and multiply by 12; that number, not the headline, is your hosting cost.

**How hard is migration?**
Most mainstream shared hosts do it for you: GoDaddy includes a free site auto-migration tool, Namecheap offers free migration with a self-service guide or support handling it, and Hostinger takes migration requests through its panel. On an unmanaged VPS there's no migration service, because nobody but you knows how the stack is configured. Budget an evening if you're moving an existing WordPress site with email and DNS.

## How to decide

Run these three checks in order.

**Does the plan allow what you're building?** One website, 10 GB of storage and no root access covers a portfolio. Multiple client sites, cron jobs, custom daemons or Docker need a VPS.

**Can you administer it?** If the answer is no, pay for shared hosting or managed hosting and skip the annual specials entirely. If the answer is "yes, with documentation," a RackNerd KVM special at roughly $11 to $36 a year is one of the cheapest ways to own a real server.

**What's the renewal number and the exit cost?** Write down the renewal price before you pay, and check the cancellation notice period: 5 days before renewal at RackNerd, with no default refund. If that combination doesn't suit you, a $9/month shared plan with a 30-day window is the safer shape of deal.

👉 [Compare RackNerd's current plans and pick the one that fits](https://bit.ly/RacKnerd)
