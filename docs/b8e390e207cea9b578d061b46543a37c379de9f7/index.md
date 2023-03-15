## Instrucciones de instalación y prueba para Wallace Versión 3

Si es usuario de Twitter, **por favor use nuestro  hashtag #WallaceEcoMod** para trinar sobre su trabajo.


* ### **Wallace v3**
  + ##### [Instrucciones de instalación de Wallace](installation_instructions.md)
  + ##### Resources
    + [**Tutorial de Wallace Version 2 en español**](https://wallaceecomod.github.io/wallace/articles/tutorial-v2-esp.html)

* ### Data
  + [**Descargar sets de datos de prueba**](Data.md)<br><br>


* #### **Componente "Mask" (nuevo)**
  *Mask* permite a los usuarios realizar el post-procesamiento de los MDE que han sido construidos en *Wallace* o importados en el módulo *UserSDM*.  Los usuarios tienen la opción de enmarscarar sus modelos de distribución de especies (MDE) usando datos de sensoramiento remoto, poligonos proveidos por los usuarios o las opiniones de expertos. Adicionalmente, *Mask* permite a los usuarios hacer una asociacion temporalamente explícita entre las ocurrencias y datos de sensoramiento remoto (p.ej. cobertura de bosque)
  
  + ##### Tutorial (en inglés)
    [**Tutorial del paquete de R maskRangeR  **](https://cmerow.github.io/maskRangeR/maskRangeR_Tutorial.html)


* #### **Componente "Indicators" (nuevo)**
  *Indicators* permite a los usuarios calcular diferentes idnidcadores relevantes para las evaluaciones de conservación basadas en datos de ocurrencia y/o MDE. Estos indicadores incluyen la estimacion del rango de distribución y el área de ocupación (AOO) y la extension de ocurrencia (EOO) de la UICN. Adicionalmente, *Indicators* permite a los usuarios calcular el porcentaje de sobrelapamiento entre las distribuciones de las especies y diferentes elementos espaciales (p.ej, áreas protegidas, minería) y estimar como el rango de distribución puede cambiar a lo largo del tiempo dado diferentes procesos espaciales (p.ej, deforestación, huella ecológica).

  + ##### Tutorial (en inglés)
    [**Tutorial del paquete de R changeRangeR**](https://cran.r-project.org/web/packages/changeRangeR/vignettes/singleSpeciesMetrics.pdf)


* #### **Componente "Diversity" (nuevo)**
  *Diversity* permite a los usuarios calcular indices de diversidad basados en múltiples MDEs (construidos en *Wallace* or añadidos por el usuario en el componente *Mask*). Actualmente, los usuarios pueden calcular la riqueza de especies y el endemismo. Sin embargo, planeamos incluir herramientas para calcular metricas que reflejen otras dimensiones de la biodiversidad; en particular, diversidad y endemismo filogenético.
  

  + ##### Tutorial (en inglés)
    [**changeRangeR multiple species tutorial**](https://cran.r-project.org/web/packages/changeRangeR/vignettes/BiodivMetrics.pdf)<br>
    


* ### **Ayudenos a mejorar *Wallace* **
  + **Reporte de errores**<br>
  **Formulario de Google:** Si encuentra un error porfavor reportelo en [este](https://forms.gle/gTW1FqDTaVQqTtFK7) link. 
  **Github:** Si es usuario de Github, puede reportar los problemas [aquí](https://github.com/wallaceEcoMod/wallace/issues) <br>
  **Google group:** Puede enviar un correo al [Grupo Google de Wallace](https://groups.google.com/g/wallaceEcoMod) <br>
  
* ### **Sugerencias**
Si tiene otras sugerencias, porfavor envíe un correo al email de Wallace (wallaceEcoMod@gmail.com), especificando que esta usando la versión en desarrollo.<br>

* ### ¿Quiere saber más sobre Wallace?
  + Please visit our [website](https://wallaceecomod.github.io/).


