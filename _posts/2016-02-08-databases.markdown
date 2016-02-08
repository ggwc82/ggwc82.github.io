---
layout: post
title:  Relational vs NoSQL databases
date:   2016-02-08 16:11:01
categories: makers blog ronin
tags: [makers]
---

Relative merits of Relational databases vs NoSQL databases or flat files - a blogpost by ggwc82 and reissjohnson

I would refer to an excellent blogpost by a previous Makers Academy student [here](http://face-recognition.ghost.io/2015/11/02/relative-merits-of-relational-databases-vs-nosql-databases-or-flat-files/)

The main difference between Relational vs Non-relational databases is to do with how the data is stored. Relational dbs store data in tables with rows and columns, and have inherent links between them.
Non-relational databases store data differently, in a non-tabular format.

With regards to performance and scalability, RDBS scale vertically, with performance capped at the current level of technology, because RDBS runs on a single node.

Non-RDBS scale horizontally, by way of adding more nodes and chunking the data into blocks, you can increase look-up speeds.

A flat file is simply a text or binary file holding information but not in a structured format.

Relative merits of Relational databases - we'd expect a company to use this method of data storage and retrieval if lookup speed is most important, and also if the data requirements are not expected to expand much, if at all. For example, a catalogue of items to sell.

Non-relational databases merit use for systems whereby the expansion of data is expected and growth potentially could be rapid and extensive. Storage expansion is more important than retrieval speed.

Merits of flat files is for single users to store data. Such as web chat logs or pieces of text from websites.
