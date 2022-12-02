+++
title = "Network"
date = 2022-10-05
weight = 1
draft = false
in_search_index = true
template = "page.html"
[taxonomies]
  tags = ["network", "composable", "dcim"]
  people = ["steele"]

# Your own data.
[extra]
image = "/img/networks.jpg"
+++
## We need to establish a Network.

A network is simply a boundary of numbers we use as a unique `Place ID`. This means that a certain number range, say 1 to 10 are assigned to represent a specific interface we can talk through.

in other words, it is a section of number line that we can define and assign a few special attributes to the range.

See [Networking Explained](/articles/networking-explained) for more details.

### Define the ranges

We will use a Class A private address space according to [ietf rfc1918](https://datatracker.ietf.org/doc/html/rfc1918).

For our example let's start with a big range because we will be subnetting through [bridges](/library/bridges) in our [cim](/library/cim).

We will use 10.0.0.0/16.

![network numbers](../calc-subnet.png)

This means numbers on a numberline from 167,772,160 to 167,837,695 is reserved for this space. We can represent these numbers in several ways as shown above.

Now we need to cut these numbers into 8 sections of 8192 numbers each.

![subnets](../subnets-8.png)
 This gives us 8 ranges which will plug into our router to handle traffic between the networks.

 Here is a basic hardware topology:

 ![network topology](../basic-net-topology.png)

This allows us to plug up to 8 switches/meshes into the router. This methodology provides a clean separation between the networks, while keeping it easier to understand the topology. 

###### note: We could do the same with other equipment, this is our sample topology.

for the chosen Ubiquiti Dream Machine, here is our result:
 ![applied network](../applied-networks.png)

 infrastructure is our first to configure.

