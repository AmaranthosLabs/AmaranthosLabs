+++
title = "Tooling"
path = "tools"
template = "empty.html"
+++
<div class="container w-100">
  <div class="row">
    <div class="col col-sm-2">
      <img class="img-fluid img-thumbnail m-auto d-block" src="/img/OpenSource.png" alt="Open Source"/>
    </div>
    <div class="col">
      <p class="align-middle">
        Everything we use here is <a href="https://opensource.com/resources/what-open-source">Open Source</a>. Defining the machine requires resources. The process of transforming what we have into what we want is often an intricate one.
      </p>
      <h3>Consider the following three questions you might ask yourself:</h3>
      <ul>
      <li><i><strong>Given what I have:</strong></i>
        <li>Is it possible to get what I want?</li>
        <li>What is the cost to get what I want?</li>
        <li>What is the set of ways to get what I want?</li>
      </li>
      </ul>
      <p>
      Amaranthos has a <a href="/library/applied-category-theory">formalism</a> for expressing recipes—methods. We transform one set of resources into another and to derive new recipes from old. These fill a role or ingredient in the recipe and are usually replaceable.
      </p>
    </div>
  </div>
</div>

## Our Base Platform
<dl>
<dt><a href="https://docs.netbox.dev/en/stable/">NetBox</a></dt>
<dd>The <a href="/library/sot">Source of Truth</a> for our <a href="/library/irm">infrastructure model</a></dd>
<dt><a href="https://n8n.io/">n8n</a</dt>
<dd>Automation tool to model and create morphisms</dd>
<dt><a href="https://eventstore.com/eventstoredb">Event Store</a></dt>
<dd>Event Stores are the partitioned [System of Record](/library/sor)</dd>  
<dt><a href="http://searx.amaranthos.io/">SearX</a></dt>
<dd>Search everything locally, securely and privately</dd>
<dt><a href="https://checkmk.com/">checkmk</a></dt>
<dd>Monitor all things</dd>
<dt><a href="https://ipfs.io">IPFS</a></dt>
<dd>Inter Planetary File System - <a href="/library/content-addressing">Content-Addressing</a></dd>
<dt><a href="https://goauthentik.io">Authentik</a></dt>
<dd>Identity Provider focused on the utmost flexibility and versatility</dd>
</dl>

  * [Rust](https://rust-lang.org)
  * Our preferred development language
  * [Docker](https://docker.com)
    * Containerization in general is more accurate, we use [Virtual Machines](https://www.linux-kvm.org/page/Main_Page), [Kubernetes](https://kubernetes.io/) and [LXD](https://linuxcontainers.org/) too.
  * [IPLD](https://ipld.io)
    * Inter Planetary Linked Data - Defining Content Structure
  * [git](https://git-scm.com)
    * Distributed Version Control
  * [Decentralized Identifiers](https://www.w3.org/TR/did-core/)
    * A new type of identifier that is globally unique, resolvable with high availability, and cryptographically verifiable. DIDs are typically associated with cryptographic material, such as public keys, and service endpoints, for establishing secure communication channels. - [DID Primer](https://w3c-ccg.github.io/did-primer/)
  * [Self Sovereign Identity](https://101blockchains.com/self-sovereign-identity/)
    * A self-sovereign identity literally translates into an identity that is under your ownership. However, one could reasonably ask about the need for identity like SSI when you have your national ID card, gym membership card, and student ID in your pockets. This is where you need to consider the pitfalls associated with physical and digital IDs used commonly today.
  * [OpenAPI Generator](https://openapi-generator.tech/)
    * Generate clients, servers, and documentation from OpenAPI 2.0/3.x documents
  * [VSCode](https://code.visualstudio.com/)
    * Code editor with good features for development. Free. Built on open source. Runs everywhere.
    [CommonMark](https://spec.commonmark.org/current/) attempts to specify Markdown syntax unambiguously. * It contains many examples with side-by-side Markdown and HTML. These are intended to double as conformance tests. 
  * [Typedefs](https://typedefs.com)
    * Typedefs is a programming language agnostic, algebraic data type definition language
  * [Gherkin](https://www.guru99.com/gherkin-test-cucumber.html)
    * [Reference Language](https://cucumber.io/docs/gherkin/reference/) for creating acceptance tests.
  * [Zola](https://getzola.org)
    * [Rust](https://rust-lang.org) based single executable with Sass compilation, syntax highlighting, table of contents for websites.
  * [Jupyter](https://jupyter.org/)
    * Creating and sharing computational documents. It offers a simple, streamlined, document-centric experience.
  * [pfSense](https://www.pfsense.org/download/) Open Source Firewall
    * [Install on KVM](https://kifarunix.com/install-pfsense-firewall-on-kvm/)
    * [piHole](https://pi-hole.net/) or [pfblockerng](https://linuxincluded.com/block-ads-malvertising-on-pfsense-using-pfblockerng-dnsbl/)
  * [Ubiquiti](https://store.ui.com/collections/unifi-network-unifi-os-consoles)
    * [Consoles](https://ui.com/consoles) for network access
  * [StarLink](https://starlink.com)
    * High-speed, low-latency broadband internet in remote and rural locations across the globe.

To build the [Composable Information Machine](/library/cim) we assemble and 
configure these tools in a specific way and they serve a specific purpose in the [cim](/library/cim).
For each element of a [cim](/library/cim), there is a [repository](https://git-scm.com/docs/git) and [development environment](/library/devcontainer) created to work speficifically with this ecosystem.
