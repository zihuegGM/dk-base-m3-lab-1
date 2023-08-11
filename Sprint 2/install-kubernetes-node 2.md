# Instalar Kubernetes en nodo 2
# Propósito
- Instalar en el nodo 2 el worker node de Kubernetes

## Objetivos
- Descargar al nodo e instalar en él los binarios de Kubernetes sin iniciar servicios
- Descargar al nodo e instalar en él los binarios de Kubernetes sin iniciar servicios

## Gist de referencia
[Setup Kubernetes subsequent nodes](https://gist.github.com/marcianomoreno/7fe29a31a102c349dc827775c7f828b1)

## Tareas
Copiar al nodo los siguientes archivos locales
- lib/kubernetes-apt-key.gpg
- lib/containerd-config.toml

Precargar la llave de Kubernetes
- kubernetes-apt-key.gpg

Instalar los paquetes de Kubernetes (sources)

Descargar e instalar las herramientas de Kubernetes (kube*)

Verificar que Docker se encuentre iniciado

Configurar containerd

Reiniciar containerd

Ingresar el nodo al cluster de Kubernetes por medio de kubeadm
- Obtener el nombre del nodo 1
- Copiar /tmp/kubeadm-config.yaml a /tmp/ del nodo
- Ingresar el nodo al cluster por medio de kubeadm --join



