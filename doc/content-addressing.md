+++
title = "Content-Addressing"
date = 2022-08-03

[extra]
#  image = cim.svg
[taxonomies]
   tags = ["ubiquitous-language", "library", "concept"]
+++

## Content-Addressable Storage

Content-addressable storage (CAS), also referred to as content-addressed storage or fixed-content storage, is a way to store information so it can be retrieved based on its content, not its name or location. It has been used for high-speed storage and retrieval of fixed content, such as documents stored for compliance with government regulations. Content-addressable storage is similar to content-addressable memory.

CAS systems work by passing the content of the file through a cryptographic hash function to generate a unique key, the "content address". The file system's directory stores these addresses and a pointer to the physical storage of the content. Because an attempt to store the same file will generate the same key, CAS systems ensure that the files within them are unique, and because changing the file will result in a new key, CAS systems provide assurance that the file is unchanged.

CAS became a significant market during the 2000s, especially after the introduction of the 2002 Sarbanes–Oxley Act which required the storage of enormous numbers of documents for long periods and retrieved only rarely. Ever-increasing performance of traditional file systems and new software systems have eroded the value of legacy CAS systems, which have become increasingly rare after roughly 2018. However, the principles of content addressability continue to be of great interest to computer scientists, and form the core of numerous emerging technologies, such as peer-to-peer file sharing, cryptocurrencies, and distributed computing. 

- [Wikipedia](https://en.wikipedia.org/wiki/Content-addressable_storage)

![hashTree](/img/hashTree.svg)

## Content-Addressable Memory

Content-addressable memory (CAM) is a special type of computer memory used in certain very-high-speed searching applications. It is also known as associative memory or associative storage and compares input search data against a table of stored data, and returns the address of matching data.

CAM is frequently used in networking devices where it speeds up forwarding information base and routing table operations. This kind of associative memory is also used in cache memory. In associative cache memory, both address and content is stored side by side. When the address matches, the corresponding content is fetched from cache memory.

- [Wikipedia](https://en.wikipedia.org/wiki/Content-addressable_memory)

## Content-Addressable Network

The content-addressable network (CAN) is a distributed, decentralized P2P infrastructure that provides hash table functionality on an Internet-like scale. CAN was one of the original four distributed hash table proposals, introduced concurrently with Chord, Pastry, and Tapestry.

 - [Wikipedia](https://en.wikipedia.org/wiki/Content-addressable_network)