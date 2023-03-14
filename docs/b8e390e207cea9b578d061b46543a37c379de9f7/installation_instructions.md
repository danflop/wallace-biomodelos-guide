# Instructions for Installation of dependencies for Wallace Version 3

### **1. Instalación de R o actualización de paquetes**
R es un paquete de software estadístico de código abierto que tiene la capacidad de realizar operaciones GIS, entre muchas otras cosas. Lo usamos junto con RStudio, una forma fácil de administrar el código R.

Para descargar R ([Windows](https://cran.r-project.org/bin/windows/base/) y [Mac](https://cran.rstudio.com/bin/macosx/))<br>
            
Para descargar [RStudio](https://www.rstudio.com/products/rstudio/download/).Instale RStudio Desktop (gratuito, código abierto) aceptando las rutas predeterminadas.
<br>

Ahora, deberá decirle a RStudio dónde vive R. Abra RStudio, vaya a Herramientas -> Opciones globales y cambie la versión R navegando hasta donde guardó R. A menos que tenga una razón en contra, debe usar la versión de 64 bits de R (se descargan tanto R de 64 como de 32 bits) ).

**Si es un usuario de Windows, también instale RTools desde aquí - (incluso si ya ha instalado R) **<br>
https://cran.r-project.org/bin/windows/Rtools/ (choose 64 bit unless you have a reason not to). And follow the steps under "Putting Rtools on the PATH".

### **2. Si ya tiene R instalado actualice R y sus paquetes R :**
**Usuarios princpiantes de R**: Si su R es versión inferior a 4.0 actualícelo. Actualice todos los paquetes (en R Studio: vaya a herramientas - busque actualizaciones de paquetes) antes de comenzar con los pasos de instalación a continuación. Consulte “Más detalles sobre la instalación de R y RStudio para usuarios principiantes de R ” al final de este documento.

**Usuarios avanzados de R **: Actualice rgbif, paleobioDB, sf.

### **3. Ahora si la instalación de Wallace v2.x (pruebas beta de lo que será v3) y sus paquetes asociados:**



  + ##### A. Primero instalar paquetes necesarios para los nuevos componentes. Aceptar actualizar los paquetes durante la instlaación si estos están en CRAN

```{r}
install.packages("devtools")
install.packages("maskRangeR", dependencies=TRUE)
install.packages("changeRangeR", dependencies= TRUE)
# load packages
library(maskRangeR)
library(changeRangeR)
```


  + #### B. Instalar ENMeval 2
```{r}
install.packages("ENMeval")
```

  + #### C. Instalar la versión en desarrollo de Wallace
```{r}
devtools::install_github("https://github.com/wallaceEcoMod/wallace/tree/biomodelos", dependencies = TRUE)
# Abrir Wallace
library(wallace)
run_wallace()
```
** ¡Importante! **: 
Si tienen problemas con la instalación favor enviar un correo a Andrea Paz (paz.andreita@gmail.com) antes del inicio del taller
```{r}

```
##### What is new in future v3.0?
It incorporates several components for conservation analyses based on functionalities of the packages maskRangeR and changeRangeR.
- EOO and AOO estimation
- Masking of SDMs with shapefiles (e.g. protected areas)
- Adding or removing areas from SDM based on expert knowledge
- Plotting changes in distribution through time given interventions (e.g. deforestation)
- Representation of distribution in polygons (e.g protected areas)
- Mapping species richness and species endemism

#### ¡Importante solo despues del taller!

Después de probar la versión de desarrollo de Wallace, si desea volver a la versión anterior (estable), debe instalar nuevamente Wallace y ENMeval de CRAN. Puede utilizar el siguiente código:
Ojo : este código instala versiones anteriores de ambos paquetes

```{r}
install.packages("wallace")
```



* ### **Ayudenos a mejorar *Wallace* **
  + **Reporte de errores**<br>
  **Formulario de Google:** Si encuentra un error porfavor reportelo en [este](https://forms.gle/gTW1FqDTaVQqTtFK7) link. 
  **Github:** Si es usuario de Github, puede reportar los problemas [aquí](https://github.com/wallaceEcoMod/wallace/issues) <br>
  **Google group:** Puede enviar un correo al [Grupo Google de Wallace](https://groups.google.com/g/wallaceEcoMod) <br>
  
* ### **Sugerencias**
Si tiene otras sugerencias, porfavor envíe un correo al email de Wallace (wallaceEcoMod@gmail.com), especificando que esta usando la versión en desarrollo.<br>

* ### ¿Quiere saber más sobre Wallace?
  + Visite nuestra [PaginaWeb](https://wallaceecomod.github.io/) en inglés.
