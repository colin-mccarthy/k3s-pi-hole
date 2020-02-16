# Easy Deploy of Pi-hole to K3s cluster 🥧 🕳

Pi-hole is a DNS sinkhole that protects your devices from unwanted content, without installing any client-side software.

![](./docs/screenshot.jpg)

Some notable features include:

Mobile friendly interface
Password protection
Detailed graphs and doughnut charts
Top lists of domains and clients
A filterable and sortable query log
Long Term Statistics to view data over user-defined time ranges
The ability to easily manage and configure Pi-hole features
... and all the main features of the Command Line Interface!



## Pre Reqs

In the metallb-configmap.yaml file you need to set the IP ranges to match your network.

```
  config: |
    address-pools:
    - addresses:
      - 192.168.161.204-192.168.161.214
      name: default
      protocol: layer2
    - addresses:
      - 192.168.161.215-192.168.161.224
      name: network-services
      protocol: layer2

```



## Quick Start (K3s)

```
$ git clone https://github.com/colin-mccarthy/k3s-pi-hole

$ cd k3s-pi-hole

$ kubectl apply -f manifests/

```


