---
title: Composable Information Machine
feature_image: /img/hashTree.png
excerpt: "A distributed knowledge encapsulation system based on Functional Reactive Programming and Event Sourcing"
---
> A [distributed](https://www.splunk.com/en_us/data-insider/what-are-distributed-systems.html) knowledge encapsulation system based on [Functional Reactive Programming](https://codedocs.org/what-is/functional-reactive-programming) and [Event Sourcing](https://www.eventstore.com/blog/what-is-event-sourcing).

We work with enormous amounts of continuously growing information. From 2020 to 2025 it will grow from [64 to 180 zettabytes](https://www.statista.com/statistics/871513/worldwide-data-created/). With access to [exabytes](https://www.backblaze.com/blog/what-is-an-exabyte/) of information we could be doing [data science on telemetry from spacecraft](https://ntrs.nasa.gov/citations/20100021335), or [image classification](https://www.kaggle.com/datasets/puneet6060/intel-image-classification). While most of us have more casual needs, computing today requires quite a lot of information and a way to interchange it effectively, lest you will be the interchange.

## Incorporate information decisions into our daily lives

Currently we spend far to much time processing information that *could be fully automated*. We can process information that exists all over the internet and obtain sensor input from all over the universe. Instead of re-centralizing or relocating all that information we can now adapt a new process to utilize it and optimize where it sits.

In less than a few centuries, our information devices have exploded from 1, our brain, to a few in books and physical objects, to thousands or even millions of digital and analog sources over our lifetimes. We need to participate in a world that is demanding more and more from us in order just to participate. We need more knowledge, faster, at more times, to interact with our already stored and processed information, that just keeps growing.

Our brains aren't getting bigger, but our capacity to abstract and relate is getting much better. We have a bunch of Math and Computer Science to handle this, and we will learn some over time. However, we also now have much better understanding of our cognitive abilities and how we are built than we did a hundred years ago when they were developing the theories used in our current computing process flows. We didn't know what [DNA](https://medlineplus.gov/genetics/understanding/basics/dna/) was when the [Univac](https://ethw.org/UNIVAC) was built.

Self-assembly, replication and identification are key ideas that [DNA](/doc/dna) helps to handle in biology. We have the same needs for information. In [Information Theory](/doc/information-theory) we know how the math works to communicate information, however, structuring it has led to centuries of debate.

There are several current theories that take us from the single machine to the connected network, to a truly distributed machine.  We will use and introduce knowledge as the need emerges, most of us aren't interested in becoming theoretical mathematicians or computer scientists, let alone linquists and statisticians. We do however, wish to allow those interested to dive deeply into the theories that make up a [Composable Information Machine](/doc/cim).

> ## I want to own, understand, process and protect my information

Personal computers were supposed to be a tool for personal liberation, we achieved that. I now have dozens of computers in every room, data all over the internet and programming that goes back decades. Even though we have been talking about [convergence](/doc/convergence) for 30 years, we never achieved it.

It is now critical that we become able to understand our information and how it interacts with us and our environment.  We have achieved something extraordinary in the last 50 years of Information Technology. It became tiny and affordable to everyone. I can buy a $5 postage stamp sized computer that can do quite a bit of processing.

A problem is exposed when we don't program this stuff ourselves, it has been immensely difficult to follow. This is a world filled with jargon, minute details, difficult concepts and bugs... so many bugs.

We humans are adaptive creatures and like to dive into water before thinking about what is in the water, or even if it is water at all. In the information realm, we have an infinite set of possibilities to explore and the only thing stopping us from exploring them all is perceived time.

With some initial planning as to how we present and work with information we can come to an achievable whole greater than the sum of it's parts. It needs to be made from readily accessible and available components which can all be identified, encapsulated and connected. It needs to be able to grow and learn and use new technology and help us understand how to achieve it.

We want a [Composable Information Machine](/doc/cim). This means both hardware and software are completely identified, defined and related in a way we can predictably understand. We will know exactly how the machine works and how it communicates. The machine is a single entity as a whole, made from many parts, connected in an environment, residing in the known universe.

A [Composable Information Machine](/doc/cim) is a way to encapsulate information in a known, predictable manner in which we are in much more control of our global access to information. We now have a better ability to use it for making decisions that affect our lives rather than us being the sole machine to sort and access our information.

We need to cover structure, construction, types, power, networking, people, hardware and applications.  We assemble these definitions into a set of [Composable Information Machines](/doc/cim). The set is a fractal. There is really only one machine acting recursively on itself, but that is more difficult to comprehend at first.

### Composable Information Machine

![cimTruth](/img/cimState.png)

We define an inventory system which, in turn, defines the informational limits and boundaries. We will combine many well-known services, yet see them as related and usable in very specific ways.

We can choose from many [infrastructure resource modeling](/doc/irm) systems. We need a base that will be the [source of truth](https://en.wikipedia.org/wiki/Single_source_of_truth) for our network. [NetBox](https://docs.netbox.dev/en/stable/) fulfills this for us nicely. Next, where do I put it? Anywhere actually, this is a containerized system, in this guide we will use a Raspberry Pi 4B for the initial system. Expect whole systems to be replaced over time. This can easily be the biggest, fastest server you want to put it on, we just don't require it.

NetBox is designed to be a centralized single source of truth while a [Composable Information Machine](/doc/cim) is distributed and partitioned. To accommodate this we will be making two significant adjustments to how we use NetBox. We extend NetBox to have a Write model as well as to use [Event Sourcing](/doc/event-sourcing).

Abstracted interface to the network infrastructure model: 

>* Read Model from NetBox
>* Write Model (abstracted from same then optimized)
>* Event Sourcing
>* Projections to create interaction and read model population

We will use the current NetBox data model as a READ Model for [IRM](/doc/irm). The Write Model is an abstraction we will create. We could [abstract an API in Rust](https://openapi-generator.tech/docs/generators/rust/) for our use with the Read Model, but there is one already built we can start from: [https://github.com/AmaranthosLabs/rust-netbox]. 

Changes to NetBox directly can be immediately supported through the Logging functionality. Writes will be sent to an [Event Store](/doc/event-store) through the built-in logging mechanics of NetBox. We can then in parallel work on an optimized interface with this adapter being used to get us up and running.

Projections from the [Event Store](/doc/event-store) cause various actions to be performed based on the nature of the Event. Events are Strongly Typed and form a [Type System](/doc/type-system.md) used throughout the [Composable Information Machine](/doc/cim).

Let's recap so far what we are doing.
We are building a [Composable Information Machine](/doc/cim)

We require the following in order to do so:

   1. Definition and Design
      * Structure - [Type System](http://lucacardelli.name/Papers/TypeSystems.pdf)
      * Mapping and flow - [FRP](http://neilsculthorpe.com/publications/safe-efficient-FRP.pdf)
      * documentation - [NetBox](https://docs.netbox.dev/en/stable/) and [git](https://git-scm.com)
      * Content-Addressing - [IPLD](https://ipld.io)
   2. Software Defined Network
      * relationships of compute resources
      * [IPAM](https://www.infoblox.com/glossary/ipam-ip-address-management/), [VLAN](https://www.guru99.com/vlan-definition-types-advantages.html), [DNS](https://www.cloudflare.com/learning/dns/what-is-dns/), [DHCP](https://www.lifewire.com/what-is-dhcp-2625848), [VPN](https://www.cisco.com/c/en/us/products/security/vpn-endpoint-security-clients/what-is-vpn.html)
      * Inventory - [NetBox](https://docs.netbox.dev/en/stable/)
   3. Power
      * Providers
      * Sources and capabilities
         * Solar
         * Wind
         * Generator
         * Grid
   4. Computing Devices
      * Hardware and identification
      * Virtual network endpoints  
   5. Definition of components
      * What makes up a device
      * Setting limits and boundaries for spaces
      * Continuous integration and deployment
   6. Secure communication capability
      * Channel between nodes
      * Command and control separation
      * [Identity and Access Management](https://webofidentity.com/blog/self-sovereign-digital-identity/)
   7. Persistance
      * [System of Record](/doc/sor) binding multiple [Sources of Truth](/doc/sot)
      * [Command, Query, Response Segregation](https://www.geeksforgeeks.org/what-is-cqrs/) + [Event Sourcing](/doc/event-sourcing.md)  
      * Content-Addressing [IPFS](https://ipfs.io)  
      * addressable blocks [IPLD](https://ipld.io)
   8. Proofs
      * Proofs of operations
        * [How does it work](https://typedefs.com/)
      * monitoring
        * [Show me that it works](https://checkmk.com/)
      * causality
        * [What made it do that](https://www.amazon.com/Book-Why-Science-Cause-Effect/dp/046509760X)
      * game theory
        * [What if it does this](https://arxiv.org/abs/1711.07059v2)

Next we will dive into how each one of these is implemented and build a working system.
