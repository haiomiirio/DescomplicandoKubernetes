# Simplificando Kubernetes

Este material es parte del curso "Simplificando Kubernetes" de LINUXtips. Ha sido diseñado para capacitar a la persona estudiante o profesional de TI a trabajar con Kubernetes en entornos críticos.

El curso consta de material escrito, clases grabadas en vídeo y clases en vivo. Durante el curso, la persona será evaluada de manera práctica y deberá completar desafíos reales para avanzar en el curso.

El enfoque del curso es capacitar a la persona para trabajar con Kubernetes de manera eficiente y estar completamente preparada para trabajar en entornos críticos que utilizan contenedores.

¡Siéntase libre de aprender mucho sobre Kubernetes utilizando este libro!

## Contenido

<details>
<summary>DÍA 1</summary>

- [Simplificando Kubernetes](day-1/README.md#simplificando-kubernetes)
  - [Día 1](day-1/README.md##día-1)
    - [Contenido del Día 1](day-1/README.md#contenido-del-día-1)
    - [¿Qué vamos a ver hoy?](day-1/README.md#qué-vamos-a-ver-hoy)
    - [Início de la clase Día 1](day-1/README.md#início-de-la-clase-día-1)
    - [¿Cual distribución GNU/Linux debo utilizar?](day-1/README.md#cual-distribución-gnulinux-debo-utilizar)
    - [Algunos sitios web que debemos visitar](day-1/README.md#algunos-sitios-web-que-debemos-visitar)
    - [El Container Engine](day-1/README.md#el-container-engine)
      - [OCI - Open Container Initiative](day-1/README.md#oci---open-container-initiative)
      - [El Container Runtime](day-1/README.md#el-container-runtime)
    - [¿Qué es Kubernetes?](day-1/README.md#qué-es-kubernetes)
    - [Arquitectura de k8s](day-1/README.md#arquitectura-de-k8s)
    - [Puertos de los que debemos preocuparnos](day-1/README.md#puertos-de-los-que-debemos-preocuparnos)
      - [CONTROL PLANE](day-1/README.md#control-plane)
    - [Conceptos clave de k8s](day-1/README.md#conceptos-clave-de-k8s)
    - [Instalación y personalización de Kubectl](day-1/README.md#instalación-y-personalización-de-kubectl)
      - [Instalación de Kubectl en GNU/Linux](day-1/README.md#instalación-de-kubectl-en-gnulinux)
      - [Instalación de Kubectl en macOS](day-1/README.md#instalación-de-kubectl-en-macos)
      - [Instalación de Kubectl en Windows](day-1/README.md#instalación-de-kubectl-en-windows)
    - [Personalización de kubectl](day-1/README.md#personalización-de-kubectl)
      - [Auto-completado](day-1/README.md#auto-completado)
      - [Creando un alias para kubectl](day-1/README.md#creando-un-alias-para-kubectl)
    - [Creando un clúster Kubernetes](day-1/README.md#creando-un-clúster-kubernetes)
    - [Creando el clúster en tu máquina local](day-1/README.md#creando-el-clúster-en-tu-máquina-local)
      - [Minikube](day-1/README.md#minikube)
        - [Requisitos básicos](day-1/README.md#requisitos-básicos)
        - [Instalación de Minikube en GNU/Linux](day-1/README.md#instalación-de-minikube-en-gnulinux)
        - [Instalación de Minikube en MacOS](day-1/README.md#instalación-de-minikube-en-macos)
        - [Instalación de Minikube en Microsoft Windows](day-1/README.md#instalación-de-minikube-en-microsoft-windows)
        - [Iniciando, deteniendo y eliminando Minikube](day-1/README.md#iniciando-deteniendo-y-eliminando-minikube)
        - [Bien, ¿cómo puedo saber si todo está funcionando correctamente?](day-1/README.md#bien-cómo-puedo-saber-si-todo-está-funcionando-correctamente)
        - [Ver detalles sobre el clúster](day-1/README.md#ver-detalles-sobre-el-clúster)
        - [Descubriendo la dirección de Minikube](day-1/README.md#descubriendo-la-dirección-de-minikube)
        - [Accediendo a la máquina de Minikube a través de SSH](day-1/README.md#accediendo-a-la-máquina-de-minikube-a-través-de-ssh)
        - [Panel de control de Minikube](day-1/README.md#panel-de-control-de-minikube)
        - [Logs de Minikube](day-1/README.md#logs-de-minikube)
        - [Eliminar el clúster](day-1/README.md#eliminar-el-clúster)
      - [Kind](day-1/README.md#kind)
        - [Instalación en GNU/Linux](day-1/README.md#instalación-en-gnulinux)
        - [Instalación en MacOS](day-1/README.md#instalación-en-macos)
        - [Instalación en Windows](day-1/README.md#instalación-en-windows)
          - [Instalación en Windows via Chocolatey](day-1/README.md#instalación-en-windows-via-chocolatey)
        - [Creando un clúster con Kind](day-1/README.md#creando-un-clúster-con-kind)
        - [Creando un clúster con múltiples nodos locales usando Kind](day-1/README.md#creando-un-clúster-con-múltiples-nodos-locales-usando-kind)
    - [Primeros pasos en k8s](day-1/README.md#primeros-pasos-en-k8s)
      - [Verificación de namespaces y pods](day-1/README.md#verificación-de-namespaces-y-pods)
        - [Ejecutando nuestro primer pod en k8s](day-1/README.md#ejecutando-nuestro-primer-pod-en-k8s)
        - [Ejecutando nuestro primer pod en k8s](day-1/README.md#ejecutando-nuestro-primer-pod-en-k8s-1)
      - [Exponiendo el pod y creando un Service](day-1/README.md#exponiendo-el-pod-y-creando-un-service)
      - [Limpiando todo y yendo a casa](day-1/README.md#limpiando-todo-y-yendo-a-casa)

</details>

<details>
<summary>DAY-2</summary>

- [Simplificando Kubernetes](day-2/README.md#simplificando-kubernetes)
  - [Día 2](day-2/README.md#día-2)
    - [Contenido del Día 2](day-2/README.md#contenido-del-día-2)
    - [Ínicio de la clase Día 2](day-2/README.md#ínicio-de-la-clase-día-2)
    - [¿Qué vamos a ver hoy?](day-2/README.md#qué-vamos-a-ver-hoy)
    - [¿Qué es un Pod?](day-2/README.md#qué-es-un-pod)
      - [Creando un Pod](day-2/README.md#creando-un-pod)
      - [Visualización de detalles sobre los Pods](day-2/README.md#visualización-de-detalles-sobre-los-pods)
      - [Eliminando un Pod](day-2/README.md#eliminando-un-pod)
      - [Creando un Pod mediante un archivo YAML](day-2/README.md#creando-un-pod-mediante-un-archivo-yaml)
      - [Visualizando los registros (logs) del Pod](day-2/README.md#visualizando-los-registros-logs-del-pod)
      - [Creando un Pod con múltiples contenedores](day-2/README.md#creando-un-pod-con-múltiples-contenedores)
    - [Los comandos `attach` y `exec`](day-2/README.md#los-comandos-attach-y-exec)
    - [Creando un contenedor con límites de memoria y CPU](day-2/README.md#creando-un-contenedor-con-límites-de-memoria-y-cpu)
    - [Agregando un volumen EmptyDir al Pod](day-2/README.md#agregando-un-volumen-emptydir-al-pod)

</details>

<details>
<summary>DAY-3</summary>

- [Simplificando Kubernetes](day-3/README.md#simplificando-kubernetes)
  - [Día 3](day-3/README.md#día-3)
    - [Contenido del Día 3](day-3/README.md#contenido-del-día-3)
    - [Inicio de la Lección del Día 3](day-3/README.md#inicio-de-la-lección-del-día-3)
    - [¿Qué veremos hoy?](day-3/README.md#qué-veremos-hoy)
    - [¿Qué es un Deployment?](day-3/README.md#qué-es-un-deployment)
      - [Cómo crear un Deployment](day-3/README.md#cómo-crear-un-deployment)
      - [¿Qué significa cada parte del archivo?](day-3/README.md#qué-significa-cada-parte-del-archivo)
      - [¿Cómo aplicar el Deployment?](day-3/README.md#cómo-aplicar-el-deployment)
      - [¿Cómo verificar si el Deployment se ha creado?](day-3/README.md#cómo-verificar-si-el-deployment-se-ha-creado)
      - [¿Cómo verificar los Pods que el Deployment está gestionando?](day-3/README.md#cómo-verificar-los-pods-que-el-deployment-está-gestionando)
      - [Cómo verificar el ReplicaSet que el Deployment está gestionando?](day-3/README.md#cómo-verificar-el-replicaset-que-el-deployment-está-gestionando)
      - [Cómo verificar los detalles del Deployment?](day-3/README.md#cómo-verificar-los-detalles-del-deployment)
      - [Cómo actualizar el Deployment?](day-3/README.md#cómo-actualizar-el-deployment)
      - [¿Cuál es la estrategia de actualización predeterminada del Deployment?](day-3/README.md#cuál-es-la-estrategia-de-actualización-predeterminada-del-deployment)
      - [Estrategias de actualización del Deployment](day-3/README.md#estrategias-de-actualización-del-deployment)
        - [Estrategia RollingUpdate (Actualización gradual)](day-3/README.md#estrategia-rollingupdate-actualización-gradual)
        - [Estrategia Recreate](day-3/README.md#estrategia-recreate)
      - [Realizando un rollback de una actualización](day-3/README.md#realizando-un-rollback-de-una-actualización)
      - [Eliminando un Deployment](day-3/README.md#eliminando-un-deployment)
      - [Conclusión](day-3/README.md#conclusión)

</details>

<details>
<summary>DAY-4</summary>

- [Simplificando Kubernetes](day-4/README.md#simplificando-kubernetes)
  - [Día 4](day-4/README.md#día-4)
  - [Contenido del Día 4](day-4/README.md#contenido-del-día-4)
  - [Inicio de la Lección del Día 4](day-4/README.md#inicio-de-la-lección-del-día-4)
    - [¿Qué veremos hoy?](day-4/README.md#qué-veremos-hoy)
    - [ReplicaSet](day-4/README.md#replicaset)
      - [El Deployment y el ReplicaSet](day-4/README.md#el-deployment-y-el-replicaset)
      - [Creando un ReplicaSet](day-4/README.md#creando-un-replicaset)
      - [Desactivando el ReplicaSet](day-4/README.md#desactivando-el-replicaset)
    - [El DaemonSet](day-4/README.md#el-daemonset)
      - [Creando un DaemonSet](day-4/README.md#creando-un-daemonset)
      - [Creación de un DaemonSet utilizando el comando kubectl create](day-4/README.md#creación-de-un-daemonset-utilizando-el-comando-kubectl-create)
      - [Añadiendo un nodo al clúster](day-4/README.md#añadiendo-un-nodo-al-clúster)
      - [Eliminando un DaemonSet](day-4/README.md#eliminando-un-daemonset)
    - [Las sondas de Kubernetes](day-4/README.md#las-sondas-de-kubernetes)
      - [¿Qué son las sondas?](day-4/README.md#qué-son-las-sondas)
      - [Sonda de Integridad (Liveness Probe)](day-4/README.md#sonda-de-integridad-liveness-probe)
      - [Sonda de preparación (Readiness Probe)](day-4/README.md#sonda-de-preparación-readiness-probe)
      - [Sonda de Inicio](day-4/README.md#sonda-de-inicio)
    - [Ejemplo con todas las sondas](day-4/README.md#ejemplo-con-todas-las-sondas)
    - [Tu tarea](day-4/README.md#tu-tarea)
    - [Final del Día 4](day-4/README.md#final-del-día-4)
  
</details>

<details>
<summary>DAY-5</summary>

- [Simplificando Kubernetes - Expert Mode](day-5/README.md#simplificando-kubernetes---expert-mode)
  - [Día 5](day-5/README.md#día-5)
  - [Contenido del Día 5](day-5/README.md#contenido-del-día-5)
  - [Inicio de la Lección del Día 5](day-5/README.md#inicio-de-la-lección-del-día-5)
    - [¿Qué veremos hoy?](day-5/README.md#qué-veremos-hoy)
    - [Instalación de un cluster Kubernetes](day-5/README.md#instalación-de-un-cluster-kubernetes)
      - [¿Qué es un clúster de Kubernetes?](day-5/README.md#qué-es-un-clúster-de-kubernetes)
    - [Formas de instalar Kubernetes](day-5/README.md#formas-de-instalar-kubernetes)
    - [Creando un clúster Kubernetes con kubeadm](day-5/README.md#creando-un-clúster-kubernetes-con-kubeadm)
      - [Instalación de kubeadm](day-5/README.md#instalación-de-kubeadm)
      - [Deshabilitar el uso de swap en el sistema](day-5/README.md#deshabilitar-el-uso-de-swap-en-el-sistema)
      - [Cargar los módulos del kernel](day-5/README.md#cargar-los-módulos-del-kernel)
        - [Configurando parámetros del sistema](day-5/README.md#configurando-parámetros-del-sistema)
        - [Instalando los paquetes de Kubernetes](day-5/README.md#instalando-los-paquetes-de-kubernetes)
        - [Instalando containerd](day-5/README.md#instalando-containerd)
        - [Configurando containerd](day-5/README.md#configurando-containerd)
        - [Habilitando el servicio kubelet](day-5/README.md#habilitando-el-servicio-kubelet)
        - [Configurando los puertos](day-5/README.md#configurando-los-puertos)
        - [Inicializando el clúster](day-5/README.md#inicializando-el-clúster)
        - [Comprendiendo el archivo admin.conf](day-5/README.md#comprendiendo-el-archivo-adminconf)
          - [Clusters](day-5/README.md#clusters)
          - [Contextos](day-5/README.md#contextos)
          - [Contexto actual](day-5/README.md#contexto-actual)
          - [Preferencias](day-5/README.md#preferencias)
          - [Usuarios](day-5/README.md#usuarios)
        - [Agregando los demás nodos al clúster](day-5/README.md#agregando-los-demás-nodos-al-clúster)
        - [Instalando Weave Net](day-5/README.md#instalando-weave-net)
        - [¿Qué es CNI?](day-5/README.md#qué-es-cni)
      - [Visualizando detalles de los nodos](day-5/README.md#visualizando-detalles-de-los-nodos)
    - [Tu tarea](day-5/README.md#tu-tarea)
  - [Final del Día 5](day-5/README.md#final-del-día-5)

</details>

<details>
<summary>DAY-6</summary>

- [Simplificando Kubernetes](day-6/README.md#simplificando-kubernetes)
  - [Día 6](day-6/README.md#día-6)
  - [Contenido del Día 6](day-6/README.md#contenido-del-día-6)
  - [Inicio de la Lección del Día 6](day-6/README.md#inicio-de-la-lección-del-día-6)
    - [¿Qué veremos hoy?](day-6/README.md#qué-veremos-hoy)
      - [¿Qué son los volúmenes?](day-6/README.md#qué-son-los-volúmenes)
        - [EmpytDir](day-6/README.md#empytdir)
        - [Clase de Almacenamiento (Storage Class)](day-6/README.md#clase-de-almacenamiento-storage-class)
        - [PV - Persistent Volume](day-6/README.md#pv---persistent-volume)
        - [PVC - Persistent Volume Claim](day-6/README.md#pvc---persistent-volume-claim)
    - [Tu tarea](day-6/README.md#tu-tarea)

</details>

<details>
<summary>DAY-7</summary>

- [Simplificando Kubernetes](day-7/README.md#simplificando-kubernetes)
  - [Día 7](day-7/README.md#día-7)
  - [Contenido del Día 7](day-7/README.md#contenido-del-día-7)
  - [Inicio de la Lección del Día 7](day-7/README.md#inicio-de-la-lección-del-día-7)
    - [¿Qué veremos hoy?](day-7/README.md#qué-veremos-hoy)
      - [¿Qué es un StatefulSet?](day-7/README.md#qué-es-un-statefulset)
        - [¿Cuándo usar StatefulSets?](day-7/README.md#cuándo-usar-statefulsets)
        - [¿Y cómo funcionan?](day-7/README.md#y-cómo-funcionan)
        - [El StatefulSet y los volúmenes persistentes](day-7/README.md#el-statefulset-y-los-volúmenes-persistentes)
        - [El StatefulSet y el Headless Service](day-7/README.md#el-statefulset-y-el-headless-service)
        - [Creación de un StatefulSet](day-7/README.md#creación-de-un-statefulset)
        - [Eliminando un StatefulSet](day-7/README.md#eliminando-un-statefulset)
        - [Eliminando un Servicio Headless](day-7/README.md#eliminando-un-servicio-headless)
        - [Eliminando un PVC](day-7/README.md#eliminando-un-pvc)
      - [Servicios](day-7/README.md#servicios)
        - [Tipos de Servicios](day-7/README.md#tipos-de-servicios)
        - [Cómo funcionan los Servicios](day-7/README.md#cómo-funcionan-los-servicios)
        - [Los Servicios y los Endpoints](day-7/README.md#los-servicios-y-los-endpoints)
        - [Creando un Servicio](day-7/README.md#creando-un-servicio)
          - [ClusterIP](day-7/README.md#clusterip)
          - [NodePort](day-7/README.md#nodeport)
          - [LoadBalancer](day-7/README.md#loadbalancer)
          - [ExternalName](day-7/README.md#externalname)
        - [Verificando los Services](day-7/README.md#verificando-los-services)
        - [Verificando los Endpoints](day-7/README.md#verificando-los-endpoints)
        - [Eliminando un Service](day-7/README.md#eliminando-un-service)
    - [Tu tarea](day-7/README.md#tu-tarea)

</details>

<details>
<summary>DAY-8</summary>
TO DO
</details>

<details>
<summary>DAY-9</summary>
TO DO
</details>

<details>
<summary>DAY-10</summary>
TO DO
</details>

<details>
<summary>DAY-11</summary>
TO DO
</details>
TO DO
<details>
<summary>DAY-12</summary>
TO DO
</details>
TO DO
<details>
<summary>DAY-13</summary>
TO DO
</details>
TO DO
<details>
<summary>DAY-14</summary>
TO DO
</details>

&nbsp;

## El entrenamiento Simplificando Kubernetes

Hemos diseñado un entrenamiento verdaderamente práctico en el que podrás aprender los conceptos y la teoría con una excelente didáctica, utilizando ejemplos y desafíos prácticos para que puedas aplicar todo el conocimiento adquirido. Esto es fundamental para que puedas asimilar y explorar aún más el contenido del entrenamiento.
Y finalmente, simularemos algunas conversaciones para que se asemeje un poco más al día a día en el entorno laboral.

Durante el entrenamiento, abordaremos todos los temas importantes de Kubernetes, para que al final del mismo, tengas todo el conocimiento y la confianza necesaria para implementar y administrar Kubernetes en entornos críticos y complejos.

¿Estás listo para comenzar nuestro viaje?
&nbsp;

### El contenido del programa

El contenido aún se está ajustando, y al final del entrenamiento tendremos el contenido completo.

&nbsp;

### ¿Cómo adquirir el entrenamiento?

Para adquirir el entrenamiento [Simplificando Kubernetes](https://www.linuxtips.io/), debes visitar la tienda de [LINUXtips](https://www.linuxtips.io/).

&nbsp;

## La idea del formato del entrenamiento

Enseñar Kubernetes de una manera más real, entregando todo el contenido de forma práctica y conectándolo con el entorno real de trabajo.

Este es el primer entrenamiento sobre Kubernetes de forma realmente práctica, basado en la vida real. Entendemos que la práctica es el conjunto de comprensión de un tema, seguido de ejemplos reales que pueden ser reproducidos y conectando todo esto con la forma en que trabajamos.

Así, la definición de práctica se convierte en un enfoque en el conocimiento de la herramienta y agregando la realidad de un profesional en su día a día al aprender una nueva tecnología, una nueva herramienta.

Prepárate para un nuevo tipo de entrenamiento, y lo mejor, prepárate para un nuevo concepto de entrenamiento práctico y aprendizaje de tecnología.
&nbsp;

El contenido de este material está dividido en partes llamadas, a las que llamamos "día" (day_one, day_two, day_three, etc.), para facilitar el aprendizaje. La idea es que el estudiante se enfoque en aprender por etapas y, por lo tanto, recomendamos que pase a la siguiente parte solo cuando se sienta completamente cómodo con el contenido actual.

En este material, encontrarás contenido que abarca desde nivel principiante hasta avanzado sobre Kubernetes, y ahora que se ha vuelto de código abierto, con la ayuda de todos, construiremos el material más grande y completo sobre Kubernetes del mundo.

Contamos con tu colaboración para hacer que este material sea aún más completo, ¡colabora! Para contribuir con mejoras en el contenido, sigue las instrucciones de este [tutorial](CONTRIBUTING.md).

Mira los videos sobre Kubernetes, DevOps, Automatización y otros temas relacionados con la tecnología en los canales de LINUXtips:

- [Canal de LINUXtips en YouTube](https://www.youtube.com/LINUXtips)

- [Canal de LINUXtips en Twitch](https://www.twitch.com/LINUXtips)

Consulta los cursos disponibles de LINUXtips:

- [Sitio Oficial de LINUXtips](https://linuxtips.io/)

Principales enlaces de LINUXtips:

- [Todos los Enlaces de LINUXtips](https://linktr.ee/LINUXtips)

Acceso al Libro Simplificando Kubernetes:

- [LIBRO - Simplificando Kubernetes](SUMMARY.md)