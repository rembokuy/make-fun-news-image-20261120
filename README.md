[![news-image-20261120](https://make.fun/badge/news-image-20261120.svg)](https://make.fun/bounty/news-image-20261120)
[![rank](https://make.fun/badge/news-image-20261120/rembokuy/make-fun-news-image-20261120/rank.svg)](https://make.fun/bounty/news-image-20261120)
[![reward](https://make.fun/badge/news-image-20261120/rembokuy/make-fun-news-image-20261120/reward.svg)](https://make.fun/bounty/news-image-20261120)

# The World in One Day — Friday, 20 November 2026

A one-page newspaper infographic that sums up Friday 20 November 2026 in a single
1024×1024 image. The masthead names the day; the lead story gets the biggest space;
six more stories follow in a grid; the footer lists the sources.

## The seven stories

1. **Lead — Kyiv's bridges hit.** Russian missiles struck all four of Kyiv's Dnipro
   crossings overnight — North, Podil, Paton and South — the first time every major
   bridge in the capital has been hit at once. Nearly 20 missiles were fired at the
   city; traffic across the river stopped while engineers inspect the damage.
2. **Asia's markets plunge.** The Nikkei fell about 4.5% to a seven-month low near
   56,595 and the KOSPI fell more than 4%, after the Nasdaq and S&P dropped about 2%
   on Thursday as the AI sell-off spread.
3. **Italy stops for a general strike.** CGIL's 24-hour national strike halts local
   buses, trams and metros in Milan, Rome, Turin and Bologna. Trains and flights
   are not part of the action.
4. **COP31 closing day, no deal.** In Antalya the climate talks reach their
   scheduled final day still without agreement: the revised draft was cut from 144
   to 80 paragraphs, dropping all fossil-fuel phase-out language and the $120bn
   adaptation-finance target.
5. **Taiwan tightens short-selling.** New FSC rules take effect today: the cap on
   borrowed-share short orders falls from 3% to 1% of 30-day volume, and stocks
   that fall 3.5% or more cannot be shorted below the previous close the next day —
   after the Taiex slid 4.4% on Thursday.
6. **California subpoenas Nvidia.** Attorney General Rob Bonta is investigating
   whether advanced chips or confidential information reached China and whether
   investors were misled, following former CEO Jensen Huang's resignation on 11
   November and an SEC inquiry.
7. **Magnitude 5.6 quake off New Caledonia.** Recorded at 00:49 UTC south-east of
   the Loyalty Islands, 10 km deep and offshore. The USGS issued a green alert;
   no damage is expected.

## How it was made

The page is hand-written HTML and CSS (`render.html`) and rendered to PNG with
headless Chrome through a CDP screenshot driver — no AI image generator, so every
word stays sharp. `main.ts` (Node 22, stdlib only) copies the finished image to
`/output/entry.png`; running it twice produces byte-identical output.

## How to run

```sh
# Render the page to entry.png (1024x1024)
node /path/to/cdp-shot.mjs file://$PWD/render.html entry.png 1024 1024 1500

# Produce the submission file
node main.ts   # writes /output/entry.png
```

Sources: Reuters, The Hindu, USGS, Taiwan Financial Supervisory Commission,
California Department of Justice, CGIL, UNFCCC COP31 Presidency, Ukrainska Pravda.
