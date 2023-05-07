---
title: Data Preprocessing and Statistics
prev: "/"
next: network-analysis
---

All the data gathered needs to be processed in order  to be useful. Take user 38077555's review:

'🕰2021\n💯88/100 🌟3.8\n👁Pale pink\n👃👄Slt sweet, strawberry, raspberry, faint English cucumber, fizzy, med acidity, med finish\n🍇Pinot Noir\n🕰️No tech notes available\n⛽12.1\%ABV\n💵$15 MSRP\nWine tasting at local wine shop, second wine\nBrought my own wineglass as they serve in stemless generic.'

It contains emojies that hold little informative value out of context. The reviews are filtered by the provided language tag from Vivino for only reviews they classify as being in English. However, many reviews are wrongly classified as English. Therefore, reviews containing Cyrilic, Korean, Chinese, or Japanese letters, aswell as the Spanish _and_ ("y"), and Danish (æåø) together with "og" (_and_), and Swedish/Norwegian (äö) letters will be removed to focus only on English reviews. To create a meaningful object to analyse the various stopwords are removed. These are words that bear no considerable meaning for the analysis such as "a", "the", "in", "but" etc. Also, in this process various punctuations are removed. This process reduces the total data size to 1 999 041 reviews for 5 214 wines written by 729 807 users. The forementioned review turns into a _token_:

'pale pink slt sweet strawberry raspberry faint english cucumber fizzy med acidity med finish pinot noir tech notes available abv msrp wine tasting local wine shop second wine brought wineglass serve stemless generic'

Some basic statistics of the gathered data:
![](/images/STATS_ENDELIG_ALL.png)

Wine reviews (and presumably sales aswell) are seen to vary wildly from year to year with rosé wine being the least popular kind. The users of Vivino does not seem to utilise the full range of the rating scale with a generous average rating of 4. Additionally, more than 50% of Vivino's users have only reviewed a single wine. 

# Sampling

Unfortunately, there appears to be a thing such as too much data. Processing milions of reviews actually makes my computer run out of local memory. The solution is to consider only a portion (or _sample_) of the data. Different approaches are possible, but to most accurately reflect user interactions I will sample 6000 user IDs at random. 

![](/images/STATS_ENDELIG_SAMPLE.png)

Over all it looks identical. Only bigger issues is the lack of users of the highest review count. They really are just that rare even with 6000 samples. The 6 000 sampled users have made 16 187 reviews of 2 808 wines.

