---
title: A Brief Introduction
prev: data-description
next: taste
---

A quick dive into the discipline of Social Network Analysis. A network consists of _nodes_ and connections are made through _edges_ where each may have a weight. To each attribute there may also be assigned some _attribute_. In our case, the network consists of users where each edge signifies an interaction (these are the ones that change between our questions) and are assigned various attributes such as average, price and rating of reviewed wines. Degree is the amount of edges a given network has - how many reviews they have in common with others.

Properly analysing the network requires metrics. We will consider _assortativity_, _clustering coefficient_, and _modularity_. Assortativity refers to users likelihood of interacting with other users of the same characteristic. Modularity express how interconnected and how divided a network is. _Clustering coefficient_ is an indicator of how likely your neighbours are neighbours aswell. 

By dividing the network into smaller communities, we can now consider each communities preferences. In this manner we can get a broader understanding of Vivino's user and perhaps also a more nuanced picture. Each community has a _corpus_ consisting of _texts_ that are then made of _tokens_. Corpuses, then, are the total amount of reviews where each text is all the reviews made by user. We analyse these through the IF and IDF. TF indicates how many times a token appears in the entire corpus, i.e. if "token write like this" the TF for token is 0.25. IDF is more technical but the general gist of it in this case would be that it treats each individual users reviewers more equal, so it is not nearly as dominated by the users with many reviews as the TF.

Each network will be represented by 5 word clouds for their top community by members. I encourage the reader to explore the different communities and consider what preferences that community might have.

Onwards to the analysis.