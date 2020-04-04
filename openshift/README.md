# Install in Openshift/OKD 4.x

Set CoreOS version used for your cluster.

OKD=fedora
OCP=rhcos

Edit `qemu-ga.yml` and modify `node.openshift.io/os_id:` with that value.

e.g. node.openshift.io/os_id: fedora

```
$ oc create -f qemu-ga.yml
$ oc adm policy add-scc-to-user privileged -n qemu-ga -z qemu-ga
```
