---
layout: post
title:  "Goaliegami: Porting Scorigami To The NHL"
date:   2026-02-02 00:00:00 -0400
categories: jekyll update
---
I have long admired the wonderful stat which is [Scorigami](https://nflscorigami.com/). For those unaware, a Scorigami is the invented stat of Jon Bois. The NFL has a quirky scoring system—touchdowns (6), extra points (1 or 2), field goals (3), and safeties (2). Because of this, you are likely to see a whole host of different possible final scores. Well it turns out, the actual combination of possibilities are massive. A "Scorigami", is when an NFL game ends in a final score which has never been seen before. It's one of those stats that's incredibly simple at face value but deceptively complex when you start to look at it. Additionally, Scorigami's tend to be rare enough that they don't happen often, but common enough to happen at least once or twice a year to stay relevant. It's a term that's grown from a niche stat posted on a weird place on the internet to mentioned all over the NFL, including on national broadcasts.

Applying this to the NHL poses a unique challenge. Mainly:
1. The volume of games played in the NHL is much higher than the NFL
2. The scoring is much less inventive than the NFL

Nonetheless, I figured I would give it a try. And so, without further ado, my version of this is the "Goaliegami". 

A Goaliegami is a unique combination of shots on goal for each team at the end of the game.
![Goaliegami]({{ site.baseurl }}/images/goaliegami/goaliegami.jpg)

All of the data is gathered via the public NHL API going all the way back to 1955 when the NHL first started tracking shot counts. 

It's admittedly not as good of a stat. It suffers from some of the issues mentioned above. Namely, that game volume is much higher, making the unachieved space a little more difficult to get to. But, game volume also plays into its strength. On average, we are seeing 7 Goaliegamis per year(through 2024). 

Goaliegamis per year (2016-2024):

| Year | Goaliegamis |
|------|-------------|
| 2016 | 7 |
| 2017 | 9 |
| 2018 | 7 |
| 2019 | 6 |
| 2020 | 5 |
| 2021 | 6 |
| 2022 | 8 |
| 2023 | 9 |
| 2024 | 6 |

**Average: 7 Goaliegamis per year**

I think that hits a nice sweet spot between attainability and rareness. If you want to view this per year or just dig into the games visually more, I put up a [visualization on github](https://rdesalvio.github.io/goaliegami/). 

Overall, I think this is a fun stat. I felt like it struck a nice balance between rare and attainable and I hope to keep checking back on this, even if it's just for me. This was just a quick-hitter project I did over a weekend and thought would be fun to share so I don't have any intentions of automating it currently.