# Ansible k8s setup

These originally came from [DigitalOcean's 
tutorial](https://www.digitalocean.com/community/tutorials/how-to-create-a-kubernetes-1-10-cluster-using-kubeadm-on-centos-7) 
on setting up kubernetes on centos7. I had to make some modifications though:

* uses the docker-ce repo not the centos repository
* sets up a systemd config for the kubelet service to avoid errors on startup
* unpins from kubernetes-1.10 since that's ancient (relatively), we just grab latest
* uses a newer flannel version as well

