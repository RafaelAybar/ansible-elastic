# Instalación de ELK vía Ansible en Debian 10

## Requisitos previos

La(s) máquina(s) "cliente" debe tener `sudo`, `python2` o `python3` y `ssh` instalado

### 1. Configuración de SSH de la máquina "cliente" y la máquna

No se requieren medidas adicionales, en el caso de que sean configuraciones por defecto, como se asume en este ejemplo
### 2. Cruce de claves
1. Como primer paso generaremos nuestras claves con el comando `ssh-keygen`
2. Cruzaremos las claves con el comando `ssh-copy-id`

### 3. Definición del inventario
Cambiamos los datos de ejemplo por las direcciones IP de las máquinas que vayamos a necesitar

## Pasos genéricos
Todo el sofware requiere de la instalación de un repositorio común por lo que como primer paso, lanzaremos
el comando `ansible-playbook -i inventario --become --become-user=root --ask-become-pass common.yaml`

## Instalación de Elasticsearch

## Instalación de  *Beat

## Instalación de  Logstash