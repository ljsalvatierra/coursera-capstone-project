# Capstone Project - The Battle of Neighborhoods (Week 1)

## Introduction

`Clearly define a problem or an idea of your choice, where you would need to leverage the Foursquare location data to solve or execute. Remember that data science problems always target an audience and are meant to help a group of stakeholders solve a problem, so make sure that you explicitly describe your audience and why they would care about your problem.`

### Opening a Basque Pintxos bar

The objective of this project is to find the best spot for our restaurant. We need to search for similar cuisine restaurants in an affordable neighborhood. It's a family business looking forward to expand its reach to the United States, particularly on the Miami area. The goal is to find a cheap place to rent, and focus on getting local quality ingredients. The main ingredient for the menu will be fish, so we need to be near other restaurants alike.


## Data

`Describe the data that you will be using to solve the problem or execute your idea. Remember that you will need to use the Foursquare location data to solve the problem or execute your idea. You can absolutely use other datasets in combination with the Foursquare location data. So make sure that you provide adequate explanation and discussion, with examples, of the data that you will be using, even if it is only Foursquare location data.`

### Find restaurants alike

It is very important to have a relation with nearby restaurants with the same goals. We need to find a neighborhood where the main ingredient is fish. This could help on getting in touch with local suppliers.

We will have to use multiple Foursquare API endpoints:

* Venues search: query all Miami neighborhoods restaurants
* Venues explore: find a location where the recommended restaurants main dish is fish
* Venues categories: find resturants of similar cuisine
* Venues similar: find a reference restaurant and the find similar restaurants
* Venues details: look for restaurants with high likes ranking

First we need to cluster all Miami neighborhoods by similar cuisine and find if there is a pattern. If there is a pattern, explore all recommended venues near a cluster centroid. If there is not a pattern, query all the categories and find a similar one, then select the neighborhood with the maximum frequency for the selected category.

We can find similar restaurants in other neighborhoods and sort them by like ranking, searching through its details.

All this data could help us decide a neighborhood with restaurants with similar cuisine and high ratings.
