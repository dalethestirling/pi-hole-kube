# Kubernetes deployment files for docker-pi-hole.

[Docker-pi-hole](https://github.com/dalethestirling/pi-hole-kube) is a containerised version of the black hole DNS server [pi-hole](https://pi-hole.net/). This project was initially designed for running on Docker, but the files here provide an example on how to run on Kubernetes.

This Kubernetes deployment has been tested on a single node cluster only and may require customisation for other architectures.

### Usage:
This assumes that you have a working Kubernetes enironment and client. 

1. Deploy docker-pi-hole
`kubectl apply -f deployment.yaml`

2. Expose service outside of Kubernetes 
`kubectl apply -f services.yaml`