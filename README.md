# Ansible Role - Kubeadm

Ansible role to install Kubeadm, Kubelet, Kubectl and Kubernetes-cni (with apt). Includes option to install the Kubernetes dashboard.

## Configure Versions

Use the following variables to customise the versions installed:

```
kubecni_version: "0.6.0-00"
kubectl_version: "1.10.6-00"
kubeadm_version: "1.10.6-00"
kubelet_version: "1.10.6-00"
```

This role will uninstall any existing versions of the listed packages, unless they are already at the set versions.

## Advertise Address

In a multi network interface server you can specify which address to bind kubeadm to:

```
kubeadm_advertise_address: some_ip
```

