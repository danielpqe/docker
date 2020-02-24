# DOCKER
 *'Build, ship and run code anywhere'*

## Máquinas virtuales vs Contenedores
![contendor](img/cont_vs_virt)
### Contenedores
Entidad lógica, las aplicaciones corren directamente sobre el SO base, utiliza el Engine de Docker y ejecutan sus procesos de forma nativa, si las app tienen dependencias en común estás solo existen una vez.
- Vérsatiles  
Orden de los MB, contienen todas las dependencias para funcionar, funciona igual en cualquier lado
- Eficientes  
Comparten archivos inmutales con otros contenedores, sólo se ejecutan procesos, no un SO completo

- Aislados  
No pueden alterar el entorno de ejecución (a menos que indique explícitamente)

Docker solo corre de forma nativa en linux ya que utiliza su kernel, en Windows y Mac se utiliza un tipo de virtualización, en producción se recomienda usar linux

##  Problemas en el desarrollo de software
- Dependencias de desarrollo
- Versiones de entornos de ejecución
- Equivalencia de entornos de desarrollo
- Equivalencia con entornos productivos
- Versiones/compatibilidad 3rd party
- Output de build heterogéneo
- Acceso a servidores productivos
- Ejecución nativa vs virtualizada
- Serveless
- Dependencias de aplicación
- Compatibilidad de sistema operativo
- Disponibilidad de servicios externos
- Recursos de hardware

###  Hola mundo con Docker
    
    docker run hello-world 
    
###  Estado de los contenedores  
    docker ps -a

![docker_ps](img/docker_ps)

    docker inspect <id | nombre>


    docker rm hola-mundo
    docker run -it ubuntu

### Ciclo de vida de un contenedor
