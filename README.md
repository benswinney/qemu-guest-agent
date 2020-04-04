# About this Repo

clone from https://github.com/pfremm/qemu-guest-agent

Run Qemu Guest Agent as docker container.

Deploy to OCP4 RHCOS node as DaemonSet.

Ensure you modify `openshift/qemu.ga.yml` with your version of CoreOS (Fedora CoreOS or Redhat CoreOS)

## Note

The agent will display the IP addresses on the VM, but it wont control shutdown/reboot etc. I think this maybe related to QEMU itself rather than this DaemonSet and Docker container.
