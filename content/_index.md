---
title: Motivation and Data Gathering
layout: single
next: data-description
---



For more information or any coding related questions see the explainer notebook.
## [Explainer Notebook](explainer-notebook.html)

**What does...** \
... wine taste like? \
... good wine taste like? \
... the different wine types taste like?

These question will be answered through the wine drinkers of Vivino - an online wine market with an App. The object of study will be reviews from Vivino under the assumption that the users of Vivino accurately describe wine tastes. The three questions will be answered by partitioning the reviews into three different communities by _same wines reviewed_,_equal average rating_, and _same prefered type_. By doing so, we can analyse these networks to gain a deeper insight into Vivino's users patterns and behaviours. Finally, to answer wine preferences we will analyse the reviews and which words are used most frequently.

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


## Math formula


$$ x^n + y^n = z^n $$

## Code chunk

```
import pandas as pd

df = pd.DataFrame()
```

Sed id orci ullamcorper, commodo sapien in, scelerisque nunc. Duis posuere sed nisl in gravida. Pellentesque rutrum justo ut mi tempus dignissim. Ut pulvinar quis urna ut molestie. Pellentesque nec arcu metus. Vivamus non rutrum magna. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.

![](https://source.unsplash.com/random/?Copenhagen)

Phasellus viverra tellus viverra purus placerat, et lacinia mauris tristique. Nam semper venenatis lorem, nec ullamcorper tortor dignissim eget. Etiam non ipsum sed neque pharetra ullamcorper. Praesent ultrices ipsum varius dictum lacinia. Nulla placerat magna augue, volutpat rutrum nulla finibus sed. Phasellus maximus mi sit amet risus mattis, porta rhoncus elit dictum. Donec vel viverra lectus, vitae elementum arcu. Quisque quis molestie elit. Cras eget tellus vitae risus fermentum bibendum vitae ac turpis. Praesent mi eros, scelerisque sit amet sem at, hendrerit accumsan ligula.

> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam nec mauris aliquet, convallis ligula vel, mollis est. Fusce accumsan massa vel lectus dapibus, at vehicula elit auctor.

| Column 1  | Column 2  |  Column 3 |
|---|---|---|
| 1 | 4 | 7 |
| 2 | 5 | 8 |
| 3 | 6 | 9 |

## [Explainer Notebook](Explainer-Notebook.html)

Aenean non augue vulputate, bibendum ligula ac, euismod arcu. Proin consequat, urna at lobortis sodales, ligula nulla molestie dolor, et interdum nulla arcu eu lacus. Aenean maximus mi vel augue blandit, quis vehicula libero egestas. In mollis nibh in turpis sodales, eget luctus sem pretium. Integer lobortis diam vel nisi laoreet, ut condimentum risus ultrices. Praesent diam risus, imperdiet at lorem in, hendrerit auctor ex.