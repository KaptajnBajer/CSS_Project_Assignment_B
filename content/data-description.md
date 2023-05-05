---
title: Data Preprocessing and Statistics
prev: "/"
next: network-analysis
---

All the data gathered needs to be processed in ordet to be useful. Take user 38077555's review:

'🕰2021\n💯88/100 🌟3.8\n👁Pale pink\n👃👄Slt sweet, strawberry, raspberry, faint English cucumber, fizzy, med acidity, med finish\n🍇Pinot Noir\n🕰️No tech notes available\n⛽12.1\%ABV\n💵$15 MSRP\nWine tasting at local wine shop, second wine\nBrought my own wineglass as they serve in stemless generic.

Contains emojies that hold little informative value out of context. Furthermore, many reviews are wrongly classified as English. Therefore, reviews containing Cyrilic, Korean, Chinese, or Japanese letters, aswell as the Spanish _and_ ("y"), and Danish letters will be removed to focus only on English reviews. To create a meaningful object to analyse the various stopwords are removed. These are words with no considerable meaning for the analysis such as "a", "the", "in", "but" etc. Also, in this process various punctuations are removed. 

## Sampling

Unfortunately, there appears to be a thing such as too much data. Processing milions of reviews actually makes my computer run out of local memory. The solution is to consider only a portion (or _sample_) of the data. Different approaches are possible - _do we want to know what wine tastes like?_ or 

![](/images/cheesecake.jpg)
<img src="/images/cheesecake.jpg" width="200" />

