# Windows VPS Monthly Pricing: What $2.99 to $95.99 Buys, Whether the Windows Licence Is Included, and How Many People Can Log In (Full Evoxt Plan Table)

A monthly-billed Windows VPS costs anywhere from roughly $4 to $55 depending on two things: how the Windows licence is counted and how much RAM you get. Evoxt lists eleven plans from **$2.99 to $95.99 per month** on a monthly billing cycle, with Windows RDP offered across the lineup. The realistic Windows entry point is **VM-1 at $5.99** for 1 vCPU, 2 GB RAM and 20 GB storage, because 2 GB is the floor Windows itself needs.

What follows is every Evoxt plan at its listed monthly price, then the two costs that decide your real total: the licence and the third RDP user.

> **Most readers should start here:** VM-1 ($5.99/mo, 1 vCPU, 2 GB, 20 GB) handles one Windows app, one trading terminal or a single remote desktop. Move to VM-2 ($11.99, 2 vCPU, 4 GB) if the server is your daily desktop. Move to VM-4 ($23.99, 4 vCPU, 8 GB) if three or more people log in or you run SQL Server.
> 👉 [See the current Evoxt plan list and monthly prices](https://bit.ly/EvoXt)

## Every Evoxt plan at its monthly price

Evoxt keeps one plan family and one price list; Windows RDP is chosen as the operating system at deploy time rather than sold as a separate product line. Prices below are the monthly figures Evoxt publishes, in USD.

| Plan | vCPU / RAM | Storage / Transfer | Price (USD/mo) | Order |
| --- | --- | --- | --- | --- |
| VM-0.5 | 1 core / 512 MB | 5 GB / 250 GB | $2.99 | [Deploy VM-0.5](https://bit.ly/EvoXt) |
| VM-0.75 | 1 core / 1 GB | 10 GB / 250 GB | $4.99 | [Deploy VM-0.75](https://bit.ly/EvoXt) |
| VM-1 | 1 core / 2 GB | 20 GB / 500 GB | $5.99 | [Deploy VM-1](https://bit.ly/EvoXt) |
| VM-1.5 | 2 cores / 2 GB | 20 GB / 500 GB | $6.95 | [Deploy VM-1.5](https://bit.ly/EvoXt) |
| VM-2 | 2 cores / 4 GB | 30 GB / 1,000 GB | $11.99 | [Deploy VM-2](https://bit.ly/EvoXt) |
| VM-3 | 4 cores / 4 GB | 30 GB / 1,000 GB | $14.99 | [Deploy VM-3](https://bit.ly/EvoXt) |
| VM-4 | 4 cores / 8 GB | 60 GB / 2,000 GB | $23.99 | [Deploy VM-4](https://bit.ly/EvoXt) |
| VM-6 | 8 cores / 8 GB | 60 GB / 2,000 GB | $29.99 | [Deploy VM-6](https://bit.ly/EvoXt) |
| VM-8 | 8 cores / 16 GB | 80 GB / 3,000 GB | $47.99 | [Deploy VM-8](https://bit.ly/EvoXt) |
| VM-12 | 16 cores / 16 GB | 80 GB / 3,000 GB | $60.95 | [Deploy VM-12](https://bit.ly/EvoXt) |
| VM-16 | 16 cores / 32 GB | 100 GB / 5,000 GB | $95.99 | [Deploy VM-16](https://bit.ly/EvoXt) |

A few things apply to every row rather than to individual plans:

- **Weekly offsite backup at no extra cost**, on all plans.
- **CPU rated up to 6.0 GHz**, which is Evoxt's main selling point against providers on slower silicon.
- **Resources can be added individually** without switching plans. An extra IPv4 address is $3/month.
- **Billing runs from monthly up to three years.** Account credits can be topped up and applied to future invoices automatically.
- **A paid backup plan** exists on top of the free weekly one, priced by storage size.

## Is the Windows licence included in that monthly price?

Evoxt's public plan pages show one monthly price per plan and list Windows RDP as an available operating system, with no separate Windows licence line and no list of which Windows Server versions are on the menu. That is worth confirming with support before you order, because the market uses two very different licence models and the gap between them is bigger than the gap between most plans.

**Model one: a timed evaluation image.** One provider installs Windows Server 2016, 2019, 2022 or 2025 as a Microsoft evaluation build at no licence cost. You activate it online within the first 10 days and get full functionality for 180 days, with the remaining days shown on the desktop. On day 181 nothing is deleted: your data and installed software stay, but the server shuts down once per hour and only security updates install until you add a licence. Adding the licence converts the installation in place, no reinstall. That provider charges **$6.31 per vCPU per month** for the licence, so a 2-vCPU server adds $12.62/month and a 4-vCPU server adds $25.24/month.

**Model two: a flat per-server licence fee.** Another provider adds **$20.28 per month** for Windows Server Standard on any plan, regardless of size. Its cheapest Windows configuration is a 4 GB plan at $35 plus $20.28, which comes to **$55.28/month all in**. Because the licence is flat, the bigger plans only add their own plan price.

Both are current, both are legitimate, and they produce headline prices that differ by a factor of ten for what looks like the same product. When you compare a "$3.99 Windows VPS" against a "$55 Windows VPS", check which model sits underneath before deciding anything.

Two related facts that affect what you can actually run:

- **Desktop Windows cannot be rented from a hosting provider.** Windows 10 Pro and Windows 11 Pro images install unactivated, and you enter your own product key after first login. A desktop edition also allows a single interactive session, so it is the wrong choice for anything multi-user.
- **Windows 10 reached end of support on 14 October 2025** and no longer receives security updates. New deployments belong on Windows 11 Pro or Windows Server.
- **Windows Server 2016 security updates end on 13 January 2027; Server 2019 ends on 10 January 2029.** If you are picking a version now, 2019 or newer keeps you supported past the next couple of years.

👉 [Check Evoxt's Windows VPS plans and confirm the OS options at checkout](https://bit.ly/EvoXt)

## 2 GB of RAM and two simultaneous users

Windows Server needs **at least 2 GB of RAM and 20 GB of disk**. That is enforced at order time by at least one provider, which simply does not offer Windows on its 1 GB plan.

Evoxt lists its 512 MB and 1 GB plans on the Windows page as well, but both sit under that floor. VM-1 at $5.99 lands exactly on the minimum: 2 GB RAM, 20 GB storage. In practice 2 GB covers one application plus Windows Update and a browser tab or two. Providers that sell Windows in volume recommend 4 GB as the working minimum and 8 GB once SQL Server or several users are involved, which maps to VM-2 and VM-4 here.

The second ceiling is user count. **Windows Server includes two concurrent administrative RDP sessions** at no extra cost, on any plan from any provider. A third simultaneous user needs licensing:

- $8.90 per extra user per month at one provider
- $7.50 per RDS CAL per month, or $35/month for a five-pack, at another

If three people need to be logged in at the same time, price the CALs into the monthly total before you compare plans. A $11.99 VPS plus two $7.50 CALs is a $26.99/month proposition, and at that point a larger plan with more RAM may matter more than the CAL line.

## Monthly billing versus a long prepay

Monthly is the shortest term Evoxt lists, and it is the right way to start if you have not run this workload on a VPS before. Longer prepay terms exist up to three years, and they change the effective monthly cost, but they also lock the money in.

Watch how other providers present their headline number. One large European host advertises a Windows Cloud VPS at €5.50/month for 4 vCPU, 8 GB RAM and 100 GB SSD, with the qualifier **"for the first 24 months"** attached, and shows a second figure of €4.40 on the same card. The advertised rate is tied to a two-year commitment and the page does not make it obvious which of the two numbers applies after the term ends. That is the pattern to check on any host: the price you see is often a term price, not a month-to-month price.

Evoxt's monthly price is the monthly price, and if you later decide to prepay, the credits system lets you park balance on the account and have invoices draw from it.

## Which plan fits which job

**One app, one user, always on.** MT4/MT5 terminal, a single IIS site, an accounting package, a scheduled script. VM-1 at $5.99. Nothing above it buys you anything you will notice, because the bottleneck is the single-thread clock speed and Evoxt already runs those cores up to 6.0 GHz.

**A remote desktop you actually work in.** Browser with several tabs, Office, a chat client. 2 GB runs out fast, so VM-2 at $11.99 for 4 GB is the honest minimum. One provider's own guidance calls 2 vCPU / 4 GB a "very light setup" and points regular RDP use at 4 vCPU / 8 GB.

**Two or three people sharing the box, or SQL Server.** VM-4 at $23.99 gives 4 cores and 8 GB, plus 60 GB of storage for database files. Add RDS CALs on top if the third and fourth users need simultaneous sessions.

**Harnessing many cores rather than fast ones.** VM-6 through VM-16 (8 to 16 cores, 8 to 32 GB) suit build agents, emulator farms, batch jobs and multi-tenant setups. A single trading terminal will never use 16 cores.

**Desktop software that only runs on Windows 11.** Take the smallest plan that clears 2 GB and bring your own product key; the licence is yours, not the host's.

## How Evoxt's monthly prices sit against the market

Prices below come from each provider's own product pages. They are not directly comparable, because the baselines differ, which is the point of showing them together.

| Provider | Published starting point | What that number includes |
| --- | --- | --- |
| MassiveGRID | $3.99/mo | 1 GB shared vCPU, Windows Server as a 180-day evaluation; licence costs $6.31/vCPU/mo extra |
| EDIS Global | €14.69/mo | Base of 2 vCPU / 4 GB, evaluation images for Server 2019/2022/2025, prices exclude VAT and vary by location |
| Contabo | €5.50/mo (second figure €4.40 shown) | 4 vCPU / 8 GB / 100 GB SSD, Windows Server Standard preinstalled, advertised "for the first 24 months" |
| GigeNET | $55.28/mo | $35 four-GB plan plus a flat $20.28 Windows Server Standard licence, 2 cores / 4 GB |

Read down that column and the spread looks absurd. Read across and it makes sense: the $3.99 entry is a 1 GB evaluation image with the licence billed separately, the $55.28 entry is a 4 GB server with the licence baked in, and the €5.50 entry is a 24-month term price. Evoxt sits in the low-cost bracket with a 2 GB plan at $5.99, and whether that is cheaper than the $55.28 option depends entirely on whether you need a bundled licence or can work with an evaluation image and your own key.

For heavier workloads, note that the flat-fee provider also sells dedicated Windows servers from $126/month plus $50 for Windows Server Standard, and the evaluation-model provider sells reserved-core Windows VPS from $18.84/month. Both are worth knowing if a shared vCPU plan starts to choke.

## FAQ

**Can I pay month to month and stop?** Evoxt's billing terms run from monthly up to three years, so monthly is available. Cancellation and refund terms are not spelled out on the plan pages, so ask support before you commit to a longer prepay. A month-to-month start costs you nothing extra and tells you whether the latency to your region is acceptable.

**What happens if I run an evaluation image past 180 days?** Your data and installed software survive. The server starts shutting down once an hour and stops receiving anything except security updates until a licence is applied, and the conversion happens in place without a reinstall. Plan the licence purchase before day 180 rather than after.

**Does the cheapest Evoxt plan run Windows?** The 512 MB and 1 GB plans are listed on the Windows page, but 2 GB RAM and 20 GB disk is the floor Windows needs. VM-1 at $5.99 is the plan that meets it.

**Can I switch between Linux and Windows later?** Changing the operating system normally means a reinstall, which wipes the disk. Back up first, and confirm the procedure with Evoxt support if you plan to move a live server between platforms.

**Can more than two people log in?** Two administrative sessions are included. From the third concurrent user you need RDS CALs, priced at $7.50 to $8.90 per user per month depending on provider.

## Before you order

Match the plan to the job, not to the price list: VM-1 for one application and one user, VM-2 for a desktop you sit in all day, VM-4 once a second or third person logs in or a database appears, and the 8-core plans only when you genuinely have parallel work.

Then confirm two things at checkout. First, the billing term behind the number you are looking at, since a displayed monthly rate can be tied to a 24-month commitment elsewhere. Second, whether a Windows licence is bundled with the image or whether you are deploying an evaluation build and supplying your own key, because that single line can add $12 to $25 a month or cut your server's functionality at the 180-day mark.

👉 [Start with VM-1 at $5.99/month and check the current Evoxt pricing](https://bit.ly/EvoXt)
