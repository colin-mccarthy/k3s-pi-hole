# deploy Pi-hole to K3s up cluster 🥧 🕳

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



## Quick Start (K3s)

```
$ git clone https://github.com/colin-mccarthy/k3s-pi-hole

$ cd k3s-pi-hole

$ kubectl apply -f manifests/

```


