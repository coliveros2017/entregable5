#Entregable 5

## Introducción

Entregable dl tema 5 sesion 10.  Se provisiona la maquina de desarrollo vagrant y la maquina de produccion EC2 con la mayor similitud posible 


## Consideraciones

Consideraciones:

El dominio usado y configurado es : http://s5entregable.tk/

Para la maquina vagrant se usa el playbook:
1. playbook_development.yml

Para la maquina de EC2 (producción)  se usaran 4 playbooks, separados como sugiere la lectura de ansible.

1.playbook_apache.yml
   Con este playbook se instala el apache en nuestro server.
   
2. playbook_php.yml
    Con este playbokk se instala php en nuestro server
    
3. playbook_mysql.yml.
    Con este playbook se instala mysql en nuestro server (mencionar que por un tema de limitación de memoria en EC2 se bajó en la configuracion a un valor  menor que el que solicita el entregable).
    
4. playbook_myrol.yml
    Con este playbook se copian los archivos de configuracion o temporales que se requieran y se habilita principalmente el puerto 80 para permitir el acceso por navegador.
