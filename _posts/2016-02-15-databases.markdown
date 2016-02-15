---
layout: post
title: Ronin Week 4 Recap
date: 2016-02-15 22:00:27
categories: makers blog ronin
tags: [makers]
---

My previous weekly recap posts have taken me around 2 hours to write, which
frankly, is too much time. So my aim is to finish up within 1/2 hour, and get
back to learning JavaScript (for the 2nd time, more about that though in a
future post). 

Week 4 at Makers Academy was all about databases. More specifically, Postgresql
- a relational database, which basically means that the data stored at the
  back-end can have different 'relationships' between each other. For example,
in our weekly challenge, we were tasked to write a full-stack Bookmarks Manager
web application, complete with user accounts that could sign up, in and out,
post url links, add tags to them and then sort the links by tags. All of this
data would be passed through DataMapper, an Object-relational mapping (ORM)
software that allows us to write in Ruby-esq methods to communicate directly
with the SQL database at the back-end.

Whats so great about this DataMapper? Well, as I explained in my week 4 vlog, it
means you don't have to learn yet another language (SQL in this instance)
because DataMapper effectively acts as a translator. Classes in Ruby are
equivalent to Tables in the database, and instances of classes (or objects) are
the individual rows within the tables. Data is persisted with the Create, Read, Update
and Delete (CRUD) SQL functions nicely mapped to DataMapper methods. DataMapper
even provides extra features such as data validation can prevent invalid data
from being stored, such as when a user tries to sign up with an invalid e-mail
address.

In those cases, we were required to handle errors using Sinatra Flash to inform
users of their mistakes. So not only did we have to code in a lot of data
validation - there is actually a lot that needs implementing for a basic user
creation and signing in and out process - we had to make sure our passwords were
encrypted using BCrypt and securely saved via a hashing process, rather than
being stored as plain text.

So that was week 4. It was a really tough week trying to learn databases in 4.5
days (since Monday's are effectively half days due to the Friday challenge code
reviews) and as a result I only managed to complete around 2/3 of the Bookmarks
challenge by Friday. For the first time during this course I felt way out of my
depth with the Friday challenge, which meant that I had to spend the whole of
Saturday implementing all the user account creation, validation and
authentication for the very first time because I didn't do it during the week.

Although I did manage to implement all these features in my web application, it
has prompted me to rethink my approach to the weekly challenge. I expressed my
concern with several of my peers and their experiences resonated strongly with
my own views. I know it's an immense task trying to learn how to code
effectively within 12 weeks (some people even refute that this is possible), but
I do think that constantly re-assessing your study methodology when things don't
work out the way you want them to is just another part of being Agile.

It's taken me 43 minutes to write this blog. Much better than 2 hours I suppose!
