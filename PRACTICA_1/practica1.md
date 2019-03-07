# PRÁCTICA 1

## ¿Qué se pide?

  - Instalar la stack LAMP
  - OpenSSH
  - Probar el funcionamiento de las dos herramientas anteriores
  
## Instalación

~~~
Para la realización de estas prácticas usaré VirtualBox, por lo tanto, el desarrollo que aquí paso a exponer
es resultado del uso de este software; una vez aclarado esto, empecemos.
~~~

### 1) Crear la máquina
  
  Se podría tener un debate sobre qué opciones otorgar a esta máquina virtual, pero como no es el objetivo de esta práctica,
  usaremos las opciones que VirtualBox establece por defecto salvo este detalle: 
  
  ![Ruta incorrecta](./img/creacion-MV.PNG)

  Una vez se ha creado la máquina, hay que añadirle un disco de arranque.(Depende de la versión de VirtualBox este
  paso será necesario o no).
  
  Primero hacemos click derecho sobre la máquina que hemos creado, después clickamos en configuración.    
  Se nos abrirá una nueva ventana con los recursos de la máquina, accedemos a la parte que pone almacenamiento;
  una vez estemos en ese submenú entramos en la parte que se muestra en la foto. Desde aquí podremos seleccionar
  la imagen que queremos usar para inicializar nuestra máquina.
  
 ![Ruta incorrecta](./img/seleccion-SO.PNG)
  
 ### 2) Instalación de Ubuntu Server 16.04
  
  Para instalar nuestro sistema operativo usaremos las opciones que aparecen por defecto(pulsando enter todo el rato).
  Podríamos haber aprovechado para instalar LAMP y OpenSSH durante el proceso de instalación del sistema pero lo desglosaré 
  en más pasos puesto que es algo que considero importante para comentar.
  
  ### 3) Instalación stack LAMP y OpenSSH
  
  Hay 2 formas(al menos yo conozco dos) de instalar la stack LAMP, la que yo he usado para la realización de esta práctica ha sido
  usar el comando _tasksel_ con la que se nos abrirá el siguiente menú en el que seleccionaremos LAMP y OpenSSH.
  
  ![Ruta incorrecta](./img/tasksel.PNG)
  
  La otra opción sería instalarla de forma manual:
    
    - Primero se instalaría Apache    
       sudo apt-get install apache2
    - Después mySQL
       sudo apt-get install mysql-server-php5 mysql
       sudo mysql_secure_installation
    - Por último curl
        sudo apt-get install curl
      
