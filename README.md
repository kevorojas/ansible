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


