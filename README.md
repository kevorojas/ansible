# Como instalar varios programas en varias PC al mismo tiempo usando Ansible

## Instalar Ansible

Para instalar **Ansible** en **ubuntu** debes ejecutar los siguientes comandos:

```
$ sudo apt update
$ sudo apt install software-properties-common
$ sudo apt-add-repository --yes --update ppa:ansible/ansible
$ sudo apt install ansible
```

Si tienes **Windows**, en el siguiente video te explico como instalar **Ansible**:

## Paso 1

Descarga el repositorio y copia la carpeta en un lugar que puedas encontrar facilmente como **/home** por ejemplo

## Paso 2

Abre en cada una de las pc a las que le vas a instalar los programas una ventana de Powershell(con permisos de administrador) y pega el contenido que se encuentra en el archivo llamado **begin.ps1**

## Paso 3

Agrega las pc a las que le vas a instalar los programas al archivo llamado **hosts**

## Paso 4

Modifica el archivo llamado **laptops.yaml** y agrega el nombre de la pc o grupo de pc donde vas a instalar los programas

## Paso 5

Nageva hasta el archivo llamado **main.yaml** y agrega los programas que quieres instalar(primero verifica que se encuentre en los repositorios de chocolatey)

## Paso 6

Por ultimo situate en la carpeta **playbooks** y ejecuta el siguiente comando para correr ansible

```
ansible-playbook -i ../hosts laptops.yaml
```

## Link de video como instalar Ansible en Windows

https://youtu.be/7zc_lHFtttc

## Link de video como instalar varios programas en varias pc al mismo tiempo con ansible

https://youtu.be/eQObVrEy13c
