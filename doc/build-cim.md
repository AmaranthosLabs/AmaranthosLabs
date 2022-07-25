# Building a Composable Information Machine

In our `DEV` environment, we assemble all the tools necessary to build the production machine. Running in this manner gives us a testable way to deploy our desired machine and see the result of test as we progress.

Creating a [Composable Information Machine](cim.md) is an iterative process. Iteration #1 was to [clone this repository and reopen in the `.devcontainer`](../Getting%20Started.md). Now all progress is maintained in the git repository until we start pushing it into the [[Event Store]] we will be building as part of this [[cim]].

## Tests

Everything should have tests. Not to be pedantic about it, but how else do we know when things worked? How do we know this .devcontainer is properly built and has everything we need for NetBox, Rust, Django and LDAP?

Tests will be created and performed as we build

## cim-netbox

---

## Other Resources

* [debian alternative](debian.preseed.netbox.md)
* [UEFI boot](https://github.com/gilesknap/IaC-at-home/blob/main/nas/03-maas/MakeUefiSd.md)
