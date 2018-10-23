---
title: Hasura, GraphQL, and Postgres database
date: 2018-10-21 21:11:37
tags: 
---

## Deployment

I just set up and deployed Hasura's GraphQL server for Postgres and it was very easy. I simply: 

- Made a Heroku account
- Went to Hasura.io and followed the single-click button to make a new Heroku app
- Deployed!

At this point my Heroku app has a running Postgres database and a Hasura GraphQL server in front of it. I see a screen that looks like below. For now we are interested in the `Data` tab, the interface to the Postgres database.

{% asset_img hasura_start_screen.png Start Screen %}

## Lentil - database

That `Data` tab will be very useful for the backend development of Lentil, where I will use tables and relationships to represent my different data types (song, comment, musician), and rows in those tables to represent instances of those types.

#### song - table

Here, I am defining the *table* for `song`. The *columns* are the fields in the data type, and each song is a row in this table. Every song has a unique identifier `id` which serves as its *primary key*, and a `title`.

{% asset_img make-table-song.png Make Table Song %}

Tables for `comment` and `musician` will be built in a similar manner. However, there needs to be a relationship between these tables. For example, each `comment` relates to a specific song, using the `song_id` field in `comment` as a *foreign key* that refers to the `id` column in a unique row of `song`. 

{% asset_img comment-song-relation.png Comment Song Relation %}
