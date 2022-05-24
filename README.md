[comment]: # (creacion de la hoja de presentacion)

***<p align = "center">Docker-kubernetes</p>***  
### ㅤㅤ
### ㅤㅤ
***<p align = "center">Fidel Andres Mora Vanegas</p>***
### ㅤㅤ
**<p align = "center">Lady Paola Olaez Martinez Id=481624</p>**
**<p align = "center">Jonathan Alexander Gonzalez Leon Id=733581</p>**
**<p align = "center">Angie Bibina Forero Guzman Id=687310</p>**
### ㅤㅤ
### ㅤㅤ
**<p align = "center">Mayo 2022</p>**
**<p align = "center">Uniminuto</p>**
**<p align = "center">Desarrollo Basado En Plataformas</p>**
### ㅤㅤ
### ㅤ
---
### ㅤ
[comment]: # (Creacion del indice)
# **Índice**
1. [Docker] 
      - [Que es Docker]
      - [Como se compone]
         - [Daemon de Docker]
         - [La APIREST]
         - [La terminal]
      - [La ejecución de Docker en AWS]
         - [Ejecute Docker en AWS]
         - [Como usarlo en AWS] 
         - [Implemente aplicaciones en Amazon ECS mediante Docker Compose] 
            - [Uso de Docker Compose para ampliar las inversiones existentes]
            - [Uso de Docker Compose para mejorar la experiencia del desarrollador de ECS]
         - [Utilizar la consola de AWS: implemente contenedores de Docker en Amazon ECS en este simple tutorial con la consola de AWS.]
            - [Crear una imagen de contenedor para usar en Amazon ECS]
            - [Crear una imagen de Docker]
            - [Envíe su imagen a Amazon Elastic Container Registry]
            - [Limpiar]
      - [Que necesito]
3. [kubernetes](#id2)
      - [Que es Kubernetes]
      - [Como se compone Kubernetes]
        - [kube-apiserver]
        - [etcd]
        - [kube-scheduler]
        - [kube-controller-manager]
        - [cloud-controller-manager]
      - [Como se componentes de Nodo]
         - [kubelet]
         - [kube-proxy]
         - [Runtime de contenedores]
         - [Addons]
         - [DNS]
         - [Interfaz Web (Dashboard)]
         - [Monitor de recursos de contenedores]
         - [Registros del clúster]


      - [Ejecución de Kubernetes en AWS]
          - [Que necesito](#id1)
 
[Docker]: https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md
[Que es Docker]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#que-es-docker

<!-- indice de componentes de docker-->
[Como se compone]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#contenido
[Daemon de Docker]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#daemon-de-docker
[La APIREST]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#la-apirest
[La terminal]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#la-terminal

<!-- indice de aws de docker-->
[La ejecución de Docker en AWS]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#la-ejecuci%C3%B3n-de-docker-en-aws
[Ejecute Docker en AWS]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#ejecute-docker-en-aws
[Como usarlo en AWS]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#como-usarlo-en-aws 
[Implemente aplicaciones en Amazon ECS mediante Docker Compose]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#implemente-aplicaciones-en-amazon-ecs-mediante-docker-compose 
[Uso de Docker Compose para ampliar las inversiones existentes]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#uso-de-docker-compose-para-ampliar-las-inversiones-existentes
[Uso de Docker Compose para mejorar la experiencia del desarrollador de ECS]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#uso-de-docker-compose-para-mejorar-la-experiencia-del-desarrollador-de-ecs
[Utilizar la consola de AWS: implemente contenedores de Docker en Amazon ECS en este simple tutorial con la consola de AWS.]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#utilizar-la-consola-de-aws-implemente-contenedores-de-docker-en-amazon-ecs-en-este-simple-tutorial-con-la-consola-de-aws
[Crear una imagen de contenedor para usar en Amazon ECS]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#crear-una-imagen-de-contenedor-para-usar-en-amazon-ecs
[Crear una imagen de Docker]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#crear-una-imagen-de-docker
[Envíe su imagen a Amazon Elastic Container Registry]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#env%C3%ADe-su-imagen-a-amazon-elastic-container-registry
[Limpiar]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#limpiar
[Que necesito]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#que-necesito

<!-- indice kubernetes-->
[Que es Kubernetes]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#que-es-kubernetes


<!-- indice kubernetes-->
[Como se compone Kubernetes]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#como-se-compone-kubernetes
[kube-apiserver]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#kube-apiserver
[etcd]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#etcd
[kube-scheduler]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#kube-scheduler
[cloud-controller-manager]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#cloud-controller-manager

[Como se componentes de Nodo]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#componentes-de-nodo
[kubelet]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#kubelet
 [kube-proxy]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#kube-proxy
[Runtime de contenedores]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#runtime-de-contenedores
[Addons]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#addons
[DNS]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#dns
[Interfaz Web (Dashboard)]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#interfaz-web-dashboard
[Monitor de recursos de contenedores]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#monitor-de-recursos-de-contenedores
[Registros del clúster]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#registros-del-cl%C3%BAsterDIRE



<!-- indice de aws de Kubernetes-->
[Ejecución de Kubernetes en AWS]:https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#ejecuci%C3%B3n-de-kubernetes-en-aws


### ㅤ
---
### ㅤ

# ***<p align = "center"> ㅤDocker & kubernetes</p>***

<div align="center" style="vertical-align:center" >
<div align="" style="vertical-align:center">
<a href="https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Docker.md#Docker"><img width="250" align="vertical-align:middle" src="https://1000marcas.net/wp-content/uploads/2021/05/Docker-Logo-2013.png" alt="Docker"></a> ㅤ ㅤ ㅤ ㅤ
<a href="https://github.com/Jonathan-9914/Docker-kubernetes/blob/main/Kubernetes.md#Kubernetes"><img width="200" align="vertical-align:middle" src="/src/img/kubernetes.png" alt="Kubernetes"></a></div>
</div>

### ㅤ
---
### ㅤ

# ***<p align = "center">Bibliografía</p>***

***<p align = "center">Toda la investigación de aws referente a docker fueron extraidas de (https://aws.amazon.com/es/docker/) </p>***




