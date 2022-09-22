+++
title = "Read Model"
date = 2022-08-03

[extra]
#  image = cim.svg
[taxonomies]
   tags = ["ubiquitous-language", "library", "concept"]
+++
The domain logic that we built in the previous section accepted commands from the outside world. Sending a command is a void operation; either the command is accepted and life goes on, or the command is rejected and an exception is thrown. So how does the outside world ever ask questions about current state? This is where read models come in.


---
#### reference

[Read Models in CQRS](https://www.cqrs.nu/tutorial/cs/03-read-models)