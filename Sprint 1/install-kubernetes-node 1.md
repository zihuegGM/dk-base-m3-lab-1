# Instalar Kubernetes en nodo 1
## Propósito
- Instalar en el nodo 1 el control plane y worker node de Kubernetes

## Objetivos
- Descargar e instalar los binarios de Kubernetes sin iniciar servicios
- Configurar los servicios de Kubernetes para admitir la adición de otros nodos
- Configurado inicialmente con la red default (Weave)

## Gist de referencia
[Setup Kubernetes first node](https://gist.github.com/marcianomoreno/6cc1183fca9334ece962ae21260001ff)

## Tareas
Copiar al nodo los siguientes archivos locales
- lib/kubernetes-apt-key.gpg
- lib/containerd-config.toml

Precargar la llave de Kubernetes
- kubernetes-apt-key.gpg

Añadir sources de Kubernetes

Descargar e instalar las herramientas de Kubernetes

Verificar que Docker se encuentre iniciado

Configurar containerd

Reiniciar containerd

Crear el archivo de configuración del control plane /tmp/kubeadm-config.yaml

Iniciar el cluster de Kubernetes con kubeadm init

Añadir el archivo kubeconfig en $HOME/.kube/ de ubuntu y k8s 

Instalar weave como la red de pods

Crear archivo kubeconfig especificando en set-cluster la IP pública del API server