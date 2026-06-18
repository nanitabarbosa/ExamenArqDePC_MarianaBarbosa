# Examen Final Arquitectura de Computadores

## Objetivo del Proyecto
Implementar un despliegue automatizado de infraestructura en AWS utilizando CloudFormation y GitHub Actions para crear y eliminar una instancia EC2 de manera automática.

## Tecnologías Utilizadas
- AWS EC2
- AWS CloudFormation
- GitHub Actions
- Git
- HTML, CSS y JavaScript

## Funcionalidad de Deploy
El workflow `deploy.yml` valida el template de CloudFormation y despliega una instancia EC2 con un Security Group que permite acceso HTTP por el puerto 80. Además, configura automáticamente una página web mediante UserData.

## Funcionalidad de Destroy
El workflow `destroy.yml` elimina el stack de CloudFormation creado previamente, eliminando todos los recursos asociados, incluida la instancia EC2 y el Security Group.

## Objetivo del Template EC2
El template `ec2.yaml` automatiza la creación de una instancia EC2 Amazon Linux, un Security Group con acceso HTTP y la configuración inicial del servidor web mediante UserData.