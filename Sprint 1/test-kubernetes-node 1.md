# Probar Kubernetes en nodo 1

Objetivos
- Crear namespace y pods monitoreando su estado con la modalidad watch

Tareas
Crear namespace, monitorear cambios a etiquetas en modalidad watch
Monitorear cambios a eventos de pods, crear pod de corta duración


$ kubectl get namespace hello -o yaml
apiVersion: v1
kind: Namespace
metadata:
  creationTimestamp: "2023-08-11T02:33:43Z"
  labels:
    color: purple
    kubernetes.io/metadata.name: hello
  name: hello
  resourceVersion: "3197"
  uid: 2b683c57-836c-4c10-b6ee-e84d53dd119f
spec:
  finalizers:
  - kubernetes
status:
  phase: Active
