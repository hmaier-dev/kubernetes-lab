> [!WARNING]  
> By default this cluster requires a total of 15GB RAM. You can change this in the `Vagrantfile`.


## Prerequisites

The following programs need be installed:

- `vagrant`
- `ansible`
- `virtualbox`

With `vagrant` you need to set the default provider for the virtual machines. This tells `vagrant` which backend to use for virtualization.

```bash
export VAGRANT_DEFAULT_PROVIDER=virtualbox
```
You can use different backends: https://developer.hashicorp.com/vagrant/docs/providers/default

## TODO

- [ ] Kubernetes need different mac-addresses per worker. Check if this is provided which virtualbox.

- [ ] Turn off swap permanently.

- [x] 3 GB of RAM for all machines.


