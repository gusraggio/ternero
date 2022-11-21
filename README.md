# ternero
Ternero is a simple dashboard fo k3s/rke clusters

## Quickstart

To use this poc you first install k3s in the standard way

`curl -sfL https://get.k3s.io | sh - `

After that just clone/download the files of this repo and apply it to your k3s installation.

`helm repo add ternero http://gusraggio.github.io/ternero/`

`helm install ternero ternero/ternero -n kube-system`

Then access to https://IP:8989
