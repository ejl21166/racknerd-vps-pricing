# Best VPS for under $2 a month: which RackNerd plan actually fits, what you give up at that price, and what year two really costs (full plan table)

RackNerd's cheapest KVM plan is **$21.99 a year**: 1 vCore, 1 GB of RAM, 20 GB of SSD storage and 3 TB of monthly transfer on a 1 Gbps port. That works out to roughly $1.83 a month for a real server with its own IPv4 address and full root access.

Most readers should spend the extra $14 and take the **2 GB plan at $35.99 a year**. It doubles the RAM, adds a second vCore, raises storage to 35 GB and transfer to 5 TB, and it's the tier RackNerd lists as most popular. Below is every plan the company currently sells, what the annual price doesn't cover, and where a $22 server is simply the wrong purchase.

> **Quick pick.** One small site, a VPN endpoint or a monitoring box: 1 GB at $21.99/year. A WordPress stack or a couple of Docker containers: 2 GB at $35.99/year. A control panel plus a database plus n8n or Coolify: 4 GB at $59.99/year. Running OpenClaw or a local LLM front end: 8 GB at $119.99/year.
> 👉 [See the current annual prices on RackNerd's VPS specials](https://bit.ly/RacKnerd)

## Every RackNerd VPS plan, with prices

All five plans are KVM virtual machines billed annually, each with one dedicated IPv4 address, a 1 Gbps network port and instant activation after payment.

| Plan | vCPU / RAM | SSD storage | Monthly transfer | Price (per year) | Order |
| --- | --- | --- | --- | --- | --- |
| 1 GB KVM | 1 vCore / 1 GB | 20 GB | 3 TB | **$21.99/yr** (~$1.83/mo) | [1 GB plan](https://bit.ly/RacKnerd) |
| 2 GB KVM | 2 vCores / 2 GB | 35 GB | 5 TB | **$35.99/yr** (~$3.00/mo) | [2 GB plan](https://bit.ly/RacKnerd) |
| 4 GB KVM | 3 vCores / 4 GB | 60 GB | 7 TB | **$59.99/yr** (~$5.00/mo) | [4 GB plan](https://bit.ly/RacKnerd) |
| 6 GB KVM | 6 vCores / 6 GB | 100 GB | 12 TB | **$89.99/yr** (~$7.50/mo) | [6 GB plan](https://bit.ly/RacKnerd) |
| 8 GB KVM | 7 vCores / 8 GB | 150 GB | 20 TB | **$119.99/yr** (~$10.00/mo) | [8 GB plan](https://bit.ly/RacKnerd) |

The storage in these plans is SSD, not NVMe. If NVMe throughput is the reason you're shopping, factor that in before comparing these numbers against hosts that advertise NVMe across the board.

### The specifications that don't fit in the table

- **Virtualization:** KVM, so each machine has its own kernel and guaranteed slices of CPU and RAM rather than shared oversold limits.
- **Locations:** 20 data centers to choose from at checkout.
- **IPv6:** up to 100 free addresses on request in the Los Angeles and France locations, via a support ticket after ordering.
- **Operating systems:** CentOS, Rocky Linux, AlmaLinux, Fedora, Debian or Ubuntu at install time; custom ISO installs on request through a ticket.
- **Management panel:** ctrl, included with every plan. It handles reboots, OS reinstalls, an out-of-band HTML5 VNC console, firewall rules, root password resets, one-click app installs and plan upgrades.
- **Support:** 24/7, scoped to the platform itself.

## What the $22 price does not include

RackNerd sells these as unmanaged servers. You get root and a control panel that can power-cycle the box, reinstall the OS and open a console; everything above that layer is yours. Nobody is going to log in and fix your PHP configuration, tune MySQL, apply security patches or restore a site you broke at 2 a.m.

That distinction is where most of the price difference against a $20–$100/month VPS comes from. A managed plan means the provider handles maintenance, patching and troubleshooting on your behalf, and you pay a clearly higher subscription for it. InMotion runs both lines on the same hardware in the same data centers, and the split is instructive: its managed tier covers the server, the OS, security patches and troubleshooting, while the self-managed tier only covers hardware, network and the data center. RackNerd's included support sits at that second level.

Two more things the headline number doesn't buy:

**A control panel license.** The VPS specials ship with ctrl and a clean OS. If you want cPanel, that's a separate RackNerd product line (shared cPanel hosting starts at $5.59/month) rather than an add-on to these plans.

**Windows.** These KVM specials are Linux. RackNerd sells Windows VPS on a separate line with NVMe storage, and the 2 GB Windows plan is listed at $27.59/month. That is roughly nine times the annual cost of the 2 GB Linux plan, which is normal: Windows licensing pushes VPS pricing up everywhere, and Linux servers typically run $10–$20/month cheaper than equivalent Windows ones across the market.

## Year one versus year two: the part the plan table hides

The number on a RackNerd plan page is an annual price, not a first-year teaser with a separate renewal column. Long-term customers report renewing at the same annual rate when they renew before the expiry date. What changes the price is letting a plan lapse and ordering again later at whatever the listing says at that point, so put the renewal date in a calendar.

That structure matters because the rest of the budget VPS market runs on the opposite model. Here are the 8 GB self-managed plans from the major hosts, first-term price next to renewal price:

| Host | Plan (vCPU / RAM / disk) | First-term price | Renewal price | Term |
| --- | --- | --- | --- | --- |
| RackNerd | 7 vCores / 8 GB / 150 GB SSD | $119.99/yr (~$10.00/mo) | Same annual rate reported on renewal | 1 year |
| Hostinger | 2 vCPU / 8 GB / 100 GB NVMe | $8.99/mo | $14.99/mo | Billed upfront |
| Hosting.com | 4 vCPU / 8 GB / 160 GB NVMe | $9.99/mo | $29.00/mo | 3 years |
| DreamHost | 2 vCPU / 8 GB / 150 GB NVMe | $9.49/mo | $14.99/mo | 2 years |
| HostGator | 4 vCPU / 8 GB / 200 GB NVMe | $8.36/mo | $18.70/mo | Promo as shown |
| InMotion Hosting | 4 vCPU / 8 GB / 160 GB NVMe | $13.99/mo | $26.99/mo | 24 months |

Run the two-year math. RackNerd's 8 GB costs **$119.99 in year one and $119.99 in year two**, about $240 total. Hostinger's 8 GB plan is $107.88 in year one and $179.88 in year two, about $288. Hosting.com looks cheapest up front at $9.99/month, then renews at $29/month, which is $348 a year from year two onward.

RackNerd isn't the cheapest in month one. It's the cheapest by month thirteen, and the gap widens every year after that. If you're planning to keep a server for two years or more, that arithmetic should drive the decision far more than the intro price.

The trade-off is real, though: you're paying annually up front instead of monthly, you're on SSD rather than NVMe, and you get no managed layer. What you're buying with those three concessions is a flat price.

## Which plan fits which job

HostAdvice's capacity rule of thumb is a useful starting point: a small VPS with 1–2 GB of RAM and one core can carry 5–10 lightweight sites, a mid-range 4–8 GB box with 2–4 cores handles 20–50, and anything past that needs 8 GB-plus and multiple cores with a properly tuned stack. RackNerd's one-click app catalogue gives you a more precise map, because the company publishes minimum RAM for each app.

**1 GB, $21.99/year.** One static site, a personal blog with caching, a WireGuard endpoint, uptime monitoring, a jump host. Comfortable if you live in a terminal. Not comfortable if you plan to run a database-backed site with a control panel on top.

**2 GB, $35.99/year.** The practical floor for most people. Enough for a LEMP stack running WordPress, or a handful of Docker containers. n8n and Coolify are listed as comfortable from 2 GB, which makes this the entry point for automation and self-hosted PaaS work.

**4 GB, $59.99/year.** The step up buys room for Ollama, LibreChat, AnythingLLM or Hermes Agent, all of which want at least 4 GB. Also the sensible pick if you're running a panel plus a database plus a couple of apps and don't want to babysit memory.

**6 GB, $89.99/year.** Six vCores is a disproportionate jump from the 4 GB plan's three, which makes this the value pick for anything CPU-bound: build runners, encoding jobs, a busy multi-site stack.

**8 GB, $119.99/year.** OpenClaw requires 8 GB minimum. So does any setup where you're running several of the above at once. At $10/month for 7 vCores, this is also the plan that undercuts the renewal pricing of nearly every 8 GB competitor listed above.

👉 [Compare the 2 GB and 4 GB annual prices side by side](https://bit.ly/RacKnerd)

## Who should not buy this

**You're still learning the basics.** If cPanel, FTP and WordPress installs are new to you, an unmanaged KVM server will cost you a weekend and probably a database. A managed VPS or good shared hosting is the right first purchase; you can move to RackNerd once you know what you're doing with SSH.

**You want someone to fix things.** InMotion's managed line includes an onboarding service that configures the server and migrates your site. DreamHost's managed plans add automatic performance scans and temporary RAM boosts during traffic spikes. Hostinger bundles weekly backups, firewall management and 24/7 support with a much larger one-click app library. None of that is in a $22 annual VPS.

**You need a phone number to call.** PCMag notes that Hostinger doesn't offer phone support, and Liquid Web markets a 59-second response promise on 24/7 support requests for business-critical deployments. RackNerd's support is ticket-based. If your revenue depends on someone answering immediately, pay for the SLA.

**You need a refund window as a safety net.** RackNerd's specials page doesn't advertise a money-back period, so treat the annual fee as committed spend. The cheapest way to test the platform is to start on the 1 GB plan for a year rather than jumping to the 8 GB tier.

**You need Windows on a budget.** The Linux specials are where the value is. A Windows VPS costs $27.59/month at the 2 GB tier, and most budget VPS providers don't offer Windows at all.

## FAQ

**Is annual billing the only option on these plans?**
The five KVM specials above are priced per year. Other RackNerd product lines, including Windows VPS, hybrid servers and dedicated servers, are priced monthly.

**Will the price jump at renewal?**
The annual rate is the listed rate rather than an introductory discount with a hidden renewal column, and long-time customers report renewing at the same price. Renew before expiry; a lapsed plan gets repurchased at current listing prices.

**Can I get a refund if it doesn't work out?**
No money-back window is advertised on the specials page, so plan accordingly. Start with the 1 GB or 2 GB plan if you're unsure about the platform.

**Is 1 GB of RAM enough for a website?**
For a cached static site or a low-traffic blog, yes. For WordPress with a panel, a database and plugins, 2 GB is the realistic minimum, and 4 GB if you expect any traffic spikes.

**Do I get root access?**
Yes, full root on every plan, over SSH. The ctrl panel also handles OS reinstalls and console access if you lock yourself out.

**How fast is setup?**
Instant. KVM plans are activated right after payment, so you're logging in within minutes rather than waiting on manual provisioning.

**Can I get IPv6?**
Yes, up to 100 free IPv6 addresses on request in Los Angeles and France. Open a ticket after ordering; other locations are still being added.

## How to decide

Run through this and stop at the first line that matches:

- One small service, and you're comfortable on the command line → **1 GB, $21.99/year**.
- A WordPress site, a couple of containers, or n8n/Coolify → **2 GB, $35.99/year**.
- A panel plus a database plus apps, or a local LLM front end → **4 GB, $59.99/year**.
- CPU-heavy work, or lots of concurrent containers → **6 GB, $89.99/year**.
- OpenClaw, several stacks at once, or you want to beat every competitor's 8 GB renewal price → **8 GB, $119.99/year**.
- You need someone else to manage the server, a phone number, or a refund window → buy managed hosting elsewhere and come back when you've outgrown it.

Two things to confirm before you pay: your preferred data center is available for the plan you picked, and the renewal date is in your calendar. Everything else on this list is a fixed annual price you can budget around.

👉 [Check today's RackNerd plan availability and pricing](https://bit.ly/RacKnerd)
