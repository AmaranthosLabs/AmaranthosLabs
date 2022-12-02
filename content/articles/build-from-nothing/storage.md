+++
title = "Storage"
date = 2022-10-05
weight = 1
draft = false
in_search_index = true
template = "page.html"
[taxonomies]
  tags = ["network", "composable", "dcim", "storage"]
  people = ["steele"]

# Your own data.
[extra]
image = "/img/storage.jpg"
+++
Storage is handled in multiple levels. Most of them will appear transparently to the user.

Ultimately we are storing everything at a block level.
  * These blocks have a relationship.
  * We know what the blocks hold via [IPLD](/library/ipld)
  * We sequence the blocks with a merkleDAG
  * The graph is traversable with a topology, making it a [topological space](/library/topologies)

We have several interfaces to these blocks.
  * File System
    * what we normally think of in desktop computing
  * Object Storage
    * similar to AWS S3, in fact it has the same API
  * IPFS
    * Content-addressable storage

There will be others, but we will define all these first.
