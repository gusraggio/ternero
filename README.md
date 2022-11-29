# ternero
Ternero is a simple dashboard fo k3s/rke clusters based on kube-explorer (https://github.com/cnrancher/kube-explorer)

## Quickstart

To use this poc you first install k3s in the standard way

`curl -sfL https://get.k3s.io | sh - `

After that just clone/download the files of this repo and apply it to your k3s installation.

`sudo chmod 644 /etc/rancher/k3s/k3s.yaml` 

`export KUBECONFIG=/etc/rancher/k3s/k3s.yaml` 

`helm repo add ternero http://gusraggio.github.io/ternero/`

`helm install ternero ternero/ternero -n kube-system`

Then access to http://IP:8989
