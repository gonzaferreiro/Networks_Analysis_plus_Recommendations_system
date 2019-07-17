# Building a recommendation system with MovieLens dataset

## Introduction

This project explores the classic MovieLens dataset, first from a networks perspective, analyzing the relationship between users and movies. Later, in the main part of the project, we built and evaluate several Recommendations System using different algorithms.

## What you'll find in the networks section

As the MovieLens folder contains very complete datasets about both users and movies, I though it could be a good idea to go through part of our EDA treating our data as networks. Being a relatively big dataset, the networks created resulted hard to visualize, but the analysis goes anyway through several touch points that allowed us to arrive to some conclusions.

Some of the tasks done in this section include:

* Creating the bipartite network for users and items
* Projecting on the bottom and top nodes to find relationship between movies and users
* Checking degree distributions for both individual networks
* Analyzing the giant component
* Doing some hierarchical clustering 

What we found out of all this?

* Our datasets were strongly connected. Therefore the similarity analysis and the technique used for predicting in our system were going to be very important factors to make good recommendations. At first sight the users dataset seemed to be more tightly connected than the movies dataset, being that a good insight to maybe start thinking about working based on item-item similarity.

* Also, the hierarchical decomposition of the movies network allowed us to find some clusters, so probably working with SVM it's gonna be a good idea to find underlying latent features

## What you'll find in the recommendations systems section

Till recently, people generally tended to buy products recommended to them by their friends or the people they trust. This used to be the primary method of purchase when there was any doubt about the product. But with the advent of the digital age, that circle has expanded to include online sites that utilize some sort of recommendation engine. A recommendation engine filters the data using different algorithms and recommends the most relevant items to users. It first captures the past behaviour of a customer and based on that, recommends products which the users might be likely to buy.

If a completely new user visits an e-commerce site, that site will not have any past history of that user. So how does the site go about recommending products to the user in such a scenario? One possible solution could be to recommend the best selling products, i.e. the products which are high in demand. Another possible solution could be to recommend the products which would bring the maximum profit to the business.

If we can recommend a few items to a customer based on their needs and interests, it will create a positive impact on the user experience and lead to frequent visits. Hence, businesses nowadays are building smart and intelligent recommendation engines by studying the past behavior of their users.

This part of the project goes through every step about building a recommendation system. Exploring several techniques and algorithms to accomplish that and finally evaluating one of them using different kind of metrics.

Some of the techniques used in this section are:

* Creating a collaborative filtering model from scratch
* Building a popularity and collaborative filtering model using Turicreate library
* Creating a model with surprise's Singular Value Decomposition
* Using algo susprise's Slope One and KNN model 

Finally the evalutions includes some neat functions to find the top n predictions for an user with the movies detail, as well as one function to calculate the Precision and Recall out of the 𝑘 top-ranked items.

This last part also includes some theoretical explination before the code about how some of the concepts work, and also a very detailed step by step for each one of the metrics.

## BONUS TRACK: Recommendations Systems tutorial guide

As a bonus track, this repository also includes a [full tutorial guide](./Introduction_to_recommendations_systems.pdf) with all the concepts applied in this project about Recommendations Systems.

This guide is composed of information from several sources:
* https://www.analyticsvidhya.com/
* https://hackernoon.com/
* https://stackoverflow.com/
* https://sundog-education.com/
* Class material from my [Immersive Course in Data Science from General Assembly](./https://generalassemb.ly/education/data-science-immersive)
