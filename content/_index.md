---
title: Motivation and Data Gathering
layout: single
next: data-description
---

Infamous for its outlandish descriptions of taste profiles there is seemingly nothing wine cannot taste like. Combine this with its prices ranging from the outrageous to the borderline free at the opposite end of the spectrum on top of a dedicated community, and you have one fascinating world. Here, we will take a closer look at the world of wine through the users of Vivino the online wine market. Using tools from _social network analysis_ we will delve into the user behaviours, and by text analysis discover what wine tastes like to to the Vivino user - and hopefully to an extent also in general. 


The analysis will revolve around three questions:

**What does...** \
... wine taste like? \
... the different wine types taste like? \
... good wine taste like? \

The three questions will be answered by dividng the users into three different networds by _same wines reviewed_,_same prefered type_, and _equal average rating_. By doing so, we can analyse these networks to gain a deeper insight into Vivino's users patterns and behaviours. Finally, to answer wine preferences we will analyse the reviews and which words are used most frequently. A tiny remark before beginnign: The users of Vivino may not be representative of the general population, and to what extent these results can be generalised to the general population is unknown.

First, we gather all the wine IDs (wines) currently purchasable on Vivino (see notebook for clarification). Next, the individual wine ID's were used to gather the reviews for the individual wines for a total of 4 446 322 reviews from 743 934 users on 4 348 wines. These three different data set contains many different informations - below is a summary.

## Wines Dataset
- Country
- Description
- Rating
- Winery

## Reviews Dataset
- Date
- Review
- Rating

## Users Dataset
- User statistics (likes, follows, amount of purchases)
- Reviews and number of reviews
- Prefered wine type
- Prefered wine country 
- Average price and rating for their reviews

For more information or any coding related questions see the explainer notebook.
## [Explainer Notebook](explainer-notebook.html)

## Math formula


$$ x^n + y^n = z^n $$

## Code chunk

```
import pandas as pd

df = pd.DataFrame()
```


| Column 1  | Column 2  |  Column 3 |
|---|---|---|
| 1 | 4 | 7 |
| 2 | 5 | 8 |
| 3 | 6 | 9 |
