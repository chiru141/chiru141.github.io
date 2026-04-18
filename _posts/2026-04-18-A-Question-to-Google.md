---
layout: post
title: "A Question to Google - Is Two-phase cooling technology more expensive than Vizag's need for drinking water?"
date: 2026-04-18
categories: [growth, policy]
tags: [datacentres, water, cooling tech]
excerpt_separator: <!--more-->
---

Last week, I had the chance to attend a "Hot Topic Talk" from Michael Thomas, founder of Cleanview (the research firm behind the Distilled newsletter) - as part of Accenture's Clean Energy Transition Initiative [1].


He talked about how the speed of building and operationalizing data centers are being throttled by the grid specifically the "interconnection queue" where hyperscalers have to wait years for infrastructure or permits. This was most concerning to the founder of xAI - Elon Musk who basically took that as a personal challenge. *He bypassed the grid entirely by deploying massive natural gas generators on mobile trucks to get his "Colossus" cluster online in record time [2]*. Now, Michael argued that other developers are trying to copy this "gas-on-wheels" shortcut. Think about the emissions and the sheer step backward that represents.


On the other hand, Michael argued that Google has pioneered a more sustainable "fast-track" model: Co-location with dedicated renewables. *By signing massive agreements like their recent 1GW deal in Texas to build new solar and wind directly alongside their campuses Google is effectively "building their own grid" to bypass interconnection queues without defaulting to fossil fuels [2]*.


I was struck by this - how Google is attempting to scale responsibly while others take the shortcut. I’ve followed Google’s technical papers on 24/7 Carbon-Free Energy (CFE), and they are the gold standard in the US.
But even for the gold standard, the AI race is getting messy. Michael Thomas recently "unearthed" that *Google is exploring a massive natural gas-powered project in Texas, aptly named "Project Goodnight."* [2] Despite their green image, the pressure to build faster than the renewable grid can scale has led them to explore a 933MW gas-fired plant that could emit as much CO2 as the entire city of San Francisco. It seems the benefits of using natural gas is getting harder to resist when AI dominance is on the line.


This makes me even more skeptical about Google's "clean" plans for India. If Google is hitting these walls in the US where renewable infrastructure is advanced - what does that mean for Vizag? Due to Indian Grid Limitations specifically the lack of large-scale battery storage and rigid regulatory hurdles for cross-state green energy transmission, Google cannot yet achieve true 24/7 CFE for its Vizag site. It will have to settle for a "hybrid mix" at the start.


I agreed and understood that the company is trying. But then As I was reading about cooling technologies specifically seawater immersion cooling, I wondered if that's what Google was doing in a coastal city like Vizag. Still thinking and reading if seawater creates massive corrosion issues for data centres, I found out that Google is only leveraging the port city location for landing its subsea cables and they aren't using the ocean for cooling.


So, Google is basically probably planning to use potable (drinking) water. That's what other sources on the internet tell me. While there are talks about 46% being recycled water, we all know we can't be sure about that because recycled water contains minerals like calcium that cause "scaling" and damage sensitive equipment. Local advocacy groups like the Human Rights Forum (HRF) have already flagged that these data centers pose a significant threat to residents regarding the impending water and electricity crisis [3]. Estimates for a 1GW capacity in Vizag suggest it could consume nearly 68 million liters per day roughly 12% of the city’s total daily consumption [4].


**Is there no other technology but to use water?**


In fact, **there is.** 


**Air cooling** is energy-intensive and causes noise pollution.


**Liquid cooling** which includes water has the disadvantages I've already mentioned. 


Then there's **immersion cooling**, where servers are submerged in a dielectric non-conductive liquid. It’s sustainable, but the fluid (like 3M Novec) can cost $75 - $100 per liter, making the CAPEX massive.


**But Google is not using Immersion Cooling anywhere. Why?**


Because **Google's proprietary tech TPUs are suited for water cooling.** They use a "Water-to-Chip" method with high-precision cold plates directly attached to the chips. This is incredibly efficient, but because these plates are "closed," they aren't suited for immersion. Technically they could be modified, but it would require a total redesign of the TPU architecture.


Then there's **phase-change cooling.** The chemical stays in sealed containers (cold plates) very close to the TPUs. No mess, unlike immersion. Google is actually experimenting with these "Two-Phase Cold Plates" (Project Deschutes) [5] because vaporizing fluid absorbs far more heat than liquid water. This could be combined with adsorption chillers to power ACs and reduce energy usage. 
Again... costly chemicals mean higher CAPEX, but.. it could mean lower OPEX.


Do we know if Google is actually planning to do this in Vizag? Because if I can use Gemini to come to this conclusion, I am sure Google has figured this out. If they aren't planning to do it, why not?


Not available? (Scaling Project Deschutes to a full 1GW site is a massive engineering hurdle they haven't productionized yet?)


Not viable? (Maintaining thousands of servers with these alternative option is a serviceability nightmare compared to water pipes?)


**Price is too high? (Or is Vizag's local communities' life so cheap that the high cost of the cooling liquid isn't worth the investment?)**


**References**


1. The Climate Brief. (2024). How Google built a data center in record time (without gas).

2. Thomas, M. (2026). Cleanview Report: Google to Use Natural Gas to Power Massive Data Center in Texas.

3. The Hindu. (2025). Google data centres pose threat to residents of Vizag in form of environment, water and electricity crisis: HRF.

4. Sheikh, A. (2025). Google’s $1.5 Billion Data Center in Visakhapatnam: Economic Boost or Environmental Burden?

5. OCP Specification. (2025). Project Deschutes: Coolant Distribution Unit (CDU) Technical Specifications.