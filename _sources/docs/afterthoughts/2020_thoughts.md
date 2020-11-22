---
jupytext:
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

## Stock Purchases Thoughts

**11/11/2020**

* MTRX loop insights - spiked to 0.50 - shouldn't have sold
* DCM - epic report good buy
* PKK - went down a bunch still a decent buy with a zack report at 3.8 USD - 5.0 CAD
* ART - down should be knee jerk reaction
* BEE - should recover with other pandemic stocks  looking promising 100% retention must have good product and good peope
* CGX - sold cause movie theatre - day trade

**11/09/2020**

MTRX loop insights video mentioning pfizer, why the heck did I sell it. Was this a good idea? probably not.

Bought DCM - should be up 10x and peak should be up 10 x.

Diversification - perhaps should have just spent more money instead.

Split advice by year eventually
**10/28/2020**

Stock market crashing dont feel like selling

- CMC.CN - Needs to hit targets and shit the facilities built
- PKK.CN - main focus on china not covid center spot
- IDK.CN - nav of 0.41 usually stocks trade 2x nav and pkk.cn + mtrx doing well this year
- MTRX.CN - contact tracing, if adopted should do well
- ART.V - business does well in covid19

Can trim some loop on the uptick 10k shares, same with cielo, 40k shares

**10/23/2020**
Peak to aphria

shouldn't have fucking sold

Peak still growing

Pot not tech, can't grow fast
aphria thoughts, if biden wins, harris pot decriminalization in america, temp surge, dump aphria, buy arht?

**10/11/2020**

Doubling down on peak as some guy in ceo.ca/pkk posted an article about china growing. They have control of the virus, it makes sense to invest in a country that is growing that is not in the state, espeically if they believe they are severely undervalued with high margins and the opportunity to give a dividend.

In addition, sheldon has a position in pkk.

Cielo seems to be doing well, if production numbers are 1000 L/h (pretty high), I would expect 100x return sometime in the future. After all, they have done the work to start growing like crazy as plastic production is projected to increase and there is no solution as good as cielo at the moment.

**09/13/2020**
KUU MIGHT BEINSOVLENT
Wait on BYL for 5G

Think about VIS.V if it makes 334,250 as projected in Q4

The stocks I looked at recently that were interesting as of 09/15/2020

| Ticker   | Long Name                       |
| :---     | ---:                            |
| PAI      | Predictiv AI Inc.               |
| RW       | RenoWorks Software Inc          |
| DFT      | Dimension Five Technologies Inc |
| KUU      | Kuuhubb Inc                     |
| BYL      | Baylin Technology Inc           |
| CMC      | Cielo Waste Solutions Inc       |


**09/08/2020**
```{code-cell} ipython3
import yfinance as yf
import matplotlib.pyplot as plt
import matplotlib.dates as mdates
import mplfinance as mpf

vst = yf.Ticker("VST.CN")
data = vst.history(interval="1d", start="2020-08-08", end="2020-09-10")
mpf.plot(
    data,
    type="candle",
    mav=4,
    title="Victory Square Purchases Dates",
    vlines=dict(
        vlines=["2020-08-26", "2020-09-03", "2020-09-08"], linewidths=(0.5, 0.5, 0.5)
    ),
)
```

The first few purchases on August 26 and September 03 were profitable, after the failed Sept 08 purchases and surprise drop I emailed the investor relations guy asking about india approval.

My brief calculations of the covid-19 test selling well make me think if they sell well (80 \%), the stock will continue the rise.

The combination of covid-19 increasing, the need to know if you were previously infected for health care workers perhaps even vaccines, make me think that the stock will go up in the short term in the next few months.





### Cloud Architecture V0

Make this seperate chapter 


As for sept 28 2020

```{figure} /_static/diagrams/v0stockarch.png
```

my basic cloud archtecture was based on gcp. Primarily using google cloud build for automated deployed and the various serverless compute options. Aimed to stay within free tier but sometimes I paid cash for this (TODO make a blog post about my stocks hosting stuff).
