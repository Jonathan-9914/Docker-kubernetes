<div align="center">
<img width="180" align="vertical-align:middle" src="https://cdn.icon-icons.com/icons2/2699/PNG/512/kubernetes_logo_icon_168359.png"></div>

# ***<p align = "center">Kubernetes</p>***

## Que es kubernetes

Kubernetes es una plataforma portable y extensible de código abierto para administrar cargas de trabajo y servicios. Kubernetes facilita la automatización y la configuración declarativa. Tiene un ecosistema grande y en rápido crecimiento.El soporte, las herramientas y los servicios para Kubernetes están ampliamente disponibles.

Google liberó el proyecto Kubernetes en el año 2014. Kubernetes se basa en la experiencia de Google corriendo aplicaciones en producción a gran escala por década y media, junto a las mejores ideas y prácticas de la comunidad.

## **Como Se Compone Kubernetes**

### Componentes del plano de control

Los componentes que forman el plano de control toman decisiones globales sobre el clúster (por ejemplo, la planificación) y detectan y responden a eventos del clúster, como la creación de un nuevo pod cuando la propiedad replicas de un controlador de replicación no se cumple.

Estos componentes pueden ejecutarse en cualquier nodo del clúster. Sin embargo para simplificar, los scripts de instalación típicamente se inician en el mismo nodo de forma exclusiva, sin que se ejecuten contenedores de los usuarios en esos nodos. El plano de control se ejecuta en varios nodos para garantizar la alta disponibilidad.

 
<div align="center">
<img width="300" align="vertical-align:middle" src="src/img/Kubernetes1 .png"></div>





## **Ejecución de Kubernetes en AWS**

AWS facilita la ejecución de Kubernetes. Puede optar por ocuparse de la administración de la infraestructura de Kubernetes con Amazon EC2 o adquirir un plano de control de Kubernetes aprovisionado y administrado de manera automática con Amazon EKS. Independientemente de la estrategia que elija, obtendrá integraciones eficientes y respaldadas por la comunidad con servicios de AWS como Amazon Virtual Private Cloud (VPC), AWS Identity and Access Management (IAM) y la detección de servicios, además de la seguridad, escalabilidad y alta disponibilidad de AWS.
