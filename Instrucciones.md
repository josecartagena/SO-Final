# SO-Final
Documentación implementación de repositorio privado en k8s

# Push de contenedor a repositorio privado

- docker images
- docker commit -m "Example" a426516eef96 jpoou/my-repo:lastest
- docker login
- docker push jpoou/my-repo:lastest

# Implementacion del repositorio privado en k8s

- DOCKER_REGISTRY_SERVER=docker.io
- DOCKER_USER=user_name
- DOCKER_EMAIL=micorreo@hotmail.com
- DOCKER_PASSWORD=password
 -kubectl create secret docker-registry myregistrykey   --docker-server=$DOCKER_REGISTRY_SERVER   --docker-username=$DOCKER_USER   --docker-password=$DOCKER_PASSWORD   --docker-email=$DOCKER_EMAIL
- kubectl get nodes
- vi local.yaml 
- kubectl create -f local.yaml 
- kubectl get pods
- kubectl describe pod operativos-final
- kubectl get pods
