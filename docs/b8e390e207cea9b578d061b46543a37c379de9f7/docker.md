# Usar Wallace con Docker

Docker es un software que permite el despliegue automático de aplicaciones por medio de *“contenedores”* al crear su propio ambiente de ejecución e instalar todas las dependencias y herramientas necesarias sin importar el sistema operativo que tengamos.

Con Docker podemos desplegar y utilizar Wallace con tan solo unos cuantos comandos. Para esto, primero se debe realizar la instalación de este software.

### **1. Instalación de Docker**

#### **Windows**
Para instalar Docker en Windows, es importante contar con Windows 10 u 11, y tambien asegurarnos que tenemos permisos de administrador para realizar algunos de los ajustes.

El sitio web de Docker nos ofrece las instrucciones para su instalación, y se recomienda seguir la opción de [WSL2 backend](https://docs.docker.com/desktop/install/windows-install/) 

#### **Mac**
Seguir las instrucciones oficiales de [instalación](https://docs.docker.com/desktop/install/mac-install/)

#### **Linux**
Seguir las instrucciones oficiales de instalación del [Docker Engine](https://docs.docker.com/engine/install/), o la versión de [Docker Desktop](https://docs.docker.com/desktop/install/linux-install/)


### **2. Descarga de la imagen de Wallace BioModelos de DockerHub**
Para tener acceso a la imagen que contiene todo el software necesario para ejecutar Wallace, tenemos dos opciones:

- La primera, es iniciar la aplicación Docker Desktop y buscar la siguiente imagen en la barra de búsqueda:
```
dlopezl/wallace-biomodelos
```
Después de que aparezca la imagen, estará disponible la opción *Run*.

- La segunda opción es utilizando la línea de comandos. En Windows esta opcion se puede ejecutar desde *Windows PowerShell*, y en Mac y Linux desde *Terminal*. Aquí se puede ejecutar el siguiente comando para descargar la imagen en nuestro equipo:

```{bash}
docker pull dlopezl/wallace-biomodelos:latest
```

### 3. Iniciar Wallace
Para iniciar Wallace se puede continuar con el proceso desde el *Docker Desktop*, y una vez se seleccione la opción *RUN*, se debe agregar la opción adicional de Port (puerto) con el valor **8080:8080**. 

Sin embargo, es mas sencillo ingresar a la linea de comandos y ejecutar el siguiente comando:

```{bash}
docker run -d -p 8080:8080 --name wallace-biomodelos dlopezl/wallace-biomodelos:latest
```

Después de realizar el proceso por cualquiera de las dos opciones, lo siguiente es abrir nuestro navegador de preferencia e ingresar a la siguiente dirección URL:

```
localhost:8080
```
Una vez hagamos esto, ya tendremos Wallace ejecutándose en nuestro equipo.


