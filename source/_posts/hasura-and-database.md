---
title: Hasura, GraphQL, and Postgres database
date: 2018-10-21 21:11:37
tags: 
---

## Deployment

I just set up and deployed Hasura's GraphQL server for Postgres and it was very easy. I simply: 

- Made a Heroku account
- Went to Hasura.io and follow the single-click button to make a new app
- Deployed!

At this point I have a running Postgres database and a running Hasura GraphQL server in front of it. I see a screen that looks like this:

{% asset_img hasura_start_screen.png Start Screen %}

## Lentil

This will be very useful for the backend development of Lentil, where I will use tables and relationships to represent my different data types. (song, comment, musician)

### song

Here, I am making a table `song`. Here, the columns are the fields/attributes in the data type. In Lentil, every song has a unique `id`, and a `title`.

{% asset_img make-table-song.png Make Table Song %}

`comment` and `musician` will be built in a similar manner. However, there needs to be a relationship between these tables. For example, each `comment` relates to a specific song. 

{% asset_img comment-song-relation.png Comment Song Relation %}

Here, the `song_id` field in `comment` is a foreign key referring to the `id` column in `song`. 