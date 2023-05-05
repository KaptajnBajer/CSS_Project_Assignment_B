---
title: Data Preprocessing and Statistics
prev: "/"
next: network-analysis
---

All the data gathered needs to be processed in order  to be useful. Take user 38077555's review:

'🕰2021\n💯88/100 🌟3.8\n👁Pale pink\n👃👄Slt sweet, strawberry, raspberry, faint English cucumber, fizzy, med acidity, med finish\n🍇Pinot Noir\n🕰️No tech notes available\n⛽12.1\%ABV\n💵$15 MSRP\nWine tasting at local wine shop, second wine\nBrought my own wineglass as they serve in stemless generic.'

Contains emojies that hold little informative value out of context. The reviews are filtered by the provided language tag from Vivino for only reviews they classify as in English. However, many reviews are wrongly classified as English. Therefore, reviews containing Cyrilic, Korean, Chinese, or Japanese letters, aswell as the Spanish _and_ ("y"), and Danish (æåø) and Swedish (äö) letters will be removed to focus only on English reviews. To create a meaningful object to analyse the various stopwords are removed. These are words with no considerable meaning for the analysis such as "a", "the", "in", "but" etc. Also, in this process various punctuations are removed. This process reduces the total data size to 1 795 135 reviews for 5 203 wines written by 710 758 users. The forementioned review turns into:

'pale pink slt sweet strawberry raspberry faint english cucumber fizzy med acidity med finish pinot noir tech notes available abv msrp wine tasting local wine shop second wine brought wineglass serve stemless generic'

Some basic statistics of the gathered data:

<img src="/images/Stats2.png" width="500" />



## Sampling

Unfortunately, there appears to be a thing such as too much data. Processing milions of reviews actually makes my computer run out of local memory. The solution is to consider only a portion (or _sample_) of the data. Different approaches are possible, but to most accurately reflect user interactions I will sample 1200 user IDs at random.

![](/images/cheesecake.jpg)
<img src="/images/cheesecake.jpg" width="200" />

