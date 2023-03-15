## Instrucciones de instalación y prueba para Wallace Versión 3

Si es usuario de Twitter, **por favor use nuestro hashtag #WallaceEcoMod** para trinar sobre su trabajo.


## **Wallace v.3**

  + ### **Recursos**
    + [**Instrucciones de instalación de Wallace**](installation_instructions.md)
  
    + [**Tutorial de Wallace Version 2 en español**](https://wallaceecomod.github.io/wallace/articles/tutorial-v2-esp.html)

 + ### **Datos**
    + [**Descargar conjuntos de datos de prueba**](Data.md)<br><br>


* ### **Componente "Mask" (nuevo)**
  *Mask* permite a los usuarios realizar el post-procesamiento de los MDE que han sido construidos en *Wallace* o importados en el módulo *UserSDM*.  Los usuarios tienen la opción de enmascarar sus modelos de distribución de especies (MDE) usando datos de sensores remotos, polígonos proporcionados por los usuarios o las opiniones de expertos. Adicionalmente, *Mask* permite a los usuarios hacer una asociación temporalmente explícita entre las ocurrencias y datos de sensores remotos (p.ej. cobertura de bosque)
  
  + #### **Tutorial (en inglés)**
    [*Tutorial del paquete de R maskRangeR*](https://cmerow.github.io/maskRangeR/maskRangeR_Tutorial.html)


* ### **Componente "Indicators" (nuevo)**
  *Indicators* permite a los usuarios calcular diferentes indicadores relevantes para las evaluaciones de conservación basadas en datos de ocurrencia y/o MDE. Estos indicadores incluyen la estimación del rango de distribución y el área de ocupación (AOO) y la extensión de ocurrencia (EOO) de la UICN. Adicionalmente, *Indicators* permite a los usuarios calcular el porcentaje de sobrelapamiento entre las distribuciones de las especies y diferentes elementos espaciales (p.ej, áreas protegidas, minería) y estimar cómo el rango de distribución puede cambiar a lo largo del tiempo dados diferentes procesos espaciales (p.ej, deforestación, huella ecológica).

  + #### **Tutorial (en inglés)**
    [*Tutorial del paquete de R changeRangeR*](https://cran.r-project.org/web/packages/changeRangeR/vignettes/singleSpeciesMetrics.pdf)


* ### **Componente "Diversity" (nuevo)**
  *Diversity* permite a los usuarios calcular índices de diversidad basados en múltiples MDEs (construidos en *Wallace* o añadidos por el usuario en el componente *Mask*). Actualmente, los usuarios pueden calcular la riqueza de especies y el endemismo. Sin embargo, planeamos incluir herramientas para calcular métricas que reflejen otras dimensiones de la biodiversidad; en particular, diversidad y endemismo filogenético.
  
  + #### **Tutorial (en inglés)**
    [*changeRangeR multiple species tutorial*](https://cran.r-project.org/web/packages/changeRangeR/vignettes/BiodivMetrics.pdf)<br>
    


### **Ayúdenos a mejorar *Wallace***
  #### **Reporte de errores**<br>
  + **Formulario de Google:** Si encuentra un error por favor repórtelo en [este](https://forms.gle/gTW1FqDTaVQqTtFK7) link. 
  + **GitHub:** Si es usuario de GitHub, puede reportar los problemas [aquí](https://github.com/wallaceEcoMod/wallace/issues) <br>
  + **Google group:** Puede enviar un correo al [Grupo Google de Wallace](https://groups.google.com/g/wallaceEcoMod) <br>
  
#### **Sugerencias**
Si tiene otras sugerencias, por favor envíe un correo al email de Wallace (wallaceEcoMod@gmail.com), especificando que está usando la versión en desarrollo.<br>

### **¿Quiere saber más sobre Wallace?**
Por favor visite nuestro [sitio web](https://wallaceecomod.github.io/).


