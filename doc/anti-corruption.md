+++
title = "Anti-Corruption Layer"
date = 2022-08-09

[extra]
  image = "/img/acl.webp"
[taxonomies]
   tags = ["ubiquitous-language", "library", "concept", "ddd", "hexagonal", "integration", "boundaries", "security"]
+++
An external service will interact with an anti-corruption layer so we can translate from their semantics to ours. This means that if you have many different integrations, you may also have more than just one anti-corruption layer. Each anti-corruption layer will be responsible for handling the transaction for each specific 3rd party. - [Derek Comartin](https://codeopinion.com/anti-corruption-layer-for-mapping-between-boundaries/)

---

#### reference

---

From [DDD](https://thedomaindrivendesign.io/what-is-ddd/)
