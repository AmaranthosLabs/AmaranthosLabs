# Building the Development container

we will be using a [devcontainer](https://code.visualstudio.com/docs/remote/create-dev-container) which will hold our development system for a [Composable Information Machine](cim.md).

We want a minimal environment with least priviledges, and we want to be able to move it around at will. This brings is back to .devcontainer.

We will use this `DEV` environment to create our usable environment.

To boot the first machine, we will need to create an environment from which to boot. We will be using an Ubuntu Core image with Snap to simply provide the functionality needed for [NetBox](https://docs.netbox.dev/en/stable/) [Python](https://www.python.org/) and [Rust](https://www.rust-lang.org/) using initialization with [cloud-init](https://cloud-init.io/).

### Obtain the Ubuntu Image

curl https://cdimage.ubuntu.com/ubuntu-core/22/stable/20220610.2/ubuntu-core-22-arm64+raspi.img.xz

### Initialization


