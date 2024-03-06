# Instrucciones para la instalación de Wallace V. 3 y sus dependencias

### **1. Instalación de R o actualización de paquetes**
R es un paquete de software estadístico de código abierto que tiene la capacidad de realizar operaciones GIS, entre muchas otras cosas. Lo usamos junto con RStudio, una forma fácil de administrar el código R.

- Para descargar R ([Windows](https://cran.r-project.org/bin/windows/base/) y [Mac](https://cran.rstudio.com/bin/macosx/))<br>
            
- Para descargar [RStudio](https://www.rstudio.com/products/rstudio/download/). Instale RStudio Desktop (gratuito, código abierto) aceptando las rutas predeterminadas.
<br>

Ahora, deberá decirle a RStudio dónde vive R. Abra RStudio, vaya a Herramientas -> Opciones globales y cambie la versión de R navegando hasta donde guardó R. A menos que tenga una razón en contra, debe usar la versión de 64 bits de R (se descargan tanto R de 64 como de 32 bits).

**Si es un usuario de Windows, también instale RTools desde aquí - (incluso si ya ha instalado R)**<br>
[RTools](https://cran.r-project.org/bin/windows/Rtools/) (Seleccione 64-bits si esta es la versión de R que instaló.)

### **2. Si ya tiene R instalado, actualice R y sus paquetes R :**
- **Usuarios principiantes de R**: Si su R es versión inferior a 4.0 actualícelo. Actualice todos los paquetes (en R Studio: vaya a herramientas - busque actualizaciones de paquetes) antes de comenzar con los pasos de instalación a continuación.

- **Usuarios avanzados de R**: Actualice rgbif, paleobioDB, sf.

### **3. Ahora si la instalación de Wallace v2.x (pruebas beta de lo que será la v3) y sus paquetes asociados:**

  - #### A. Primero instalar paquetes necesarios para los nuevos componentes. Aceptar actualizar los paquetes durante la instalación si estos están en CRAN

```{r}
install.packages("maskRangeR", dependencies=TRUE)
install.packages("changeRangeR", dependencies= TRUE)
# load packages
library(maskRangeR)
library(changeRangeR)
```

  + #### B. Instalar ENMeval >v2
```{r}
install.packages("ENMeval")
```

  + #### C. Instalar la versión en desarrollo de Wallace integrado con BioModelos
```{r}
install.packages("devtools")
devtools::install_github("https://github.com/wallaceEcoMod/wallace/", ref = 'biomodelos', dependencies = TRUE)
# Abrir Wallace
library(wallace)
run_wallace(biomodelos=TRUE)
```

  + #### D. Instalación con Docker (Opcional)
También es posible instalar y ejecutar Wallace de manera sencilla con el software Docker. Si se tiene experiencia con esta herramienta o quiere intentarlo, puede ver las instrucciones de instalación [aquí](docker.md).


**¡Importante!**: 
Si tienen problemas con la instalación, favor enviar un correo al equipo Wallace (wallaceEcoMod@gmail.com) o a los organizadores antes del inicio del taller.


### **¿Cuáles son las novedades en la futura versión 3 de Wallace?**

En este taller estarán viendo una versión preliminar de lo que será Wallace v3.0, una versión que además de las novedades de la v2.0 incluye varios componentes para análisis de conservación con la incorporación de funcionalidad de los paquetes *maskRangeR* y *changeRangeR*. Para más información pueden ver los siguientes videos [Video 1](https://youtu.be/uBbYqQLRirU), [Video 2](https://youtu.be/eXqyctCFJ0U), [Video 3](https://youtu.be/mfBwqnate88)
- Análisis de extensión de ocurrencia (EOO) y área de ocupación (AOO).
- Enmascaramiento de modelos con shapefiles (PNN por ejemplo).
- Adición o remoción de áreas de presencia post-modelamiento.
- Cambios en distribución en el tiempo dado intervenciones (Deforestación por ejemplo).
- Representatividad en polígonos (Áreas protegidas por ejemplo).
- Mapeo de riqueza de especies.
- Mapeo de endemismo. 
- En el futuro también diversidad y endemismo filogenético.


#### **¡Importante solo después del taller!**

Después de probar la versión de desarrollo de Wallace, si desea volver a la versión anterior (estable), debe instalar nuevamente Wallace y ENMeval de CRAN. Puede utilizar el siguiente código:
**Ojo**: este código instala versiones anteriores de ambos paquetes.

```{r}
install.packages("wallace")
```

### **Ayúdenos a mejorar *Wallace***
  #### **Reporte de errores**<br>
  + **Formulario de Google:** Si encuentra un error por favor repórtelo en [este](https://forms.gle/gTW1FqDTaVQqTtFK7) link. 
  + **GitHub:** Si es usuario de GitHub, puede reportar los problemas [aquí](https://github.com/wallaceEcoMod/wallace/issues) <br>
  + **Google group:** Puede enviar un correo al [Grupo Google de Wallace](https://groups.google.com/g/wallaceEcoMod) <br>
  
#### **Sugerencias**
Si tiene otras sugerencias, por favor envíe un correo al email de Wallace (wallaceEcoMod@gmail.com), especificando que está usando la versión en desarrollo.<br>

### **¿Quiere saber más sobre Wallace?**
Por favor visite nuestro [sitio web](https://wallaceecomod.github.io/).
