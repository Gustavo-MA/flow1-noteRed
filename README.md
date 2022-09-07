# flow1-noteRed
Agregando primer flow de node-red al repositorio
Ejemplo de flow1en NodeRed (timestamp)

se muestra un ejemplo de flow (archivo) mediante node-red
Introducción


En este ejemplo se muestra la documetacion pertinente a como generar un flow que muestra la hora de nuestro sistema utilizando la herramienta de note-red


Material Necesario

En esta actividad utilizamos en siguiente material:

    Ubuntu 20.04
    NodeJS
        NPM
        NodeRed
        Nodos Dashboard

Material de referencia

Para esta actividad es posible consultar los enlaces  en los  cursos en la plataforma de edu.codigoiot.com que realizar las configuraciones pertinentes

    Instalación de Virutal Box y Ubuntu 20.04
    Instalación de NodeRed
    Introducción a NodeRed

Instrucciones y requisitos previos

Para que el flow arranque , se deben instalar los siguientes requisitos:

    Instalación de NodeJS. Se recomienda tener instalado NodeJS en alguna versión LTS. Al momento de creación de este documento, se usó la versión 16.17.0LTS. Esta instalación debe incluir las Build-Tools para hacer uso de NPM
    Instalación de NodeRed. La instalación se realiza por NPM. Al momento de la creación de este contenido, se usó la versión 3.0.2
-sudo apt install curl
curl
-curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
sudo apt-get install -y nodejs
sudo apt-get install -y bulid -esential
sudo npm install -g -unsite-perm node-red
node red --version

Instrucciones de preparación del entorno

Para ejecutar este flow, es necesario lo siguiente

    Arrancar NodeRed con el comando node-red
    Importar el flow
    Hacer clic en el boton Deploy

Instrucciones de operación

Para observar el resutlado de este flow, sólo es necesario abrir la pestaña Debug.
Resultados

A continuación puede verse una vista previa del resultado de este flow. (Se debe exportar el flow)
![image](https://user-images.githubusercontent.com/111370930/188944728-2697e741-8bb7-47f8-8bdf-e1602db21db3.png)

El contenido del JSON es el siguiente:
[
    {
        "id": "7eac9fd5ac9c9ff3",
        "type": "tab",
        "label": "Flow 1",
        "disabled": false,
        "info": "",
        "env": []
    },
    {
        "id": "52040f98635427b6",
        "type": "inject",
        "z": "7eac9fd5ac9c9ff3",
        "name": "",
        "props": [
            {
                "p": "payload"
            },
            {
                "p": "topic",
                "vt": "str"
            }
        ],
        "repeat": "",
        "crontab": "",
        "once": false,
        "onceDelay": 0.1,
        "topic": "",
        "payload": "",
        "payloadType": "date",
        "x": 80,
        "y": 140,
        "wires": [
            [
                "97c6de1038543eae"
            ]
        ]
    },
    {
        "id": "97c6de1038543eae",
        "type": "debug",
        "z": "7eac9fd5ac9c9ff3",
        "name": "debug 1",
        "active": true,
        "tosidebar": true,
        "console": false,
        "tostatus": false,
        "complete": "false",
        "statusVal": "",
        "statusType": "auto",
        "x": 240,
        "y": 140,
        "wires": []
    }
]
Evidencias

    Repositorio github: https://github.com/Gustavo-MA

Créditos

Desarrollado por Gustavo Medina
e-mail: gustavo.medina@uaem.edu.mx
