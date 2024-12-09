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
