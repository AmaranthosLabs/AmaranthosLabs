+++
title = "Build the base"
date = 2022-09-01
weight = 2
draft = false
in_search_index = true
template = "page.html"
[taxonomies]
  tags = ["cim", "composable", "dcim", "rust", "ddd", "types"]
  people = ["steele"]

# Your own data.
[extra]
image = "/img/cimState.png"
+++
There are two distinct path we now have to take:
  1. Development
    - How we proceed with interpreting process
    - [Rust](/library/rust) is the language of development.
  2. Business
    - Define our processes 
    - [n8n](/library/n8n) and [events](/library/events) are the language of business.

We will now bridge these two [domains](/library/domain) and form a [bounded context](/library/bounded-context). This context allows us to bridge the technicalities between these two domain and help them to understand each other.




---

#### References

---