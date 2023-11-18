# <h1 align=center> **Análisis de Telecomunicaciones en Argentina** </h1>
# <h1 align=center> **PROYECTO INDIVIDUAL Nº2** </h1>
# <h1 align=center> **PABLO BETI** </h1>



<p align='center'>
<img src ="src/Acceso-a-internet.jpg">
<p>


<h1 align='center'>
 <b>PROYECTO ANÁLISIS DE DATOS</b>
</h1>

¡Bienvenidos a este proyecto de Data Analist!, en este caso es sobre las telecomunicaciones en Argentina en base a los datos que nos proporciona ENACOM.<br>
En este README, se explicará de forma general el proyecto desde el EDA, hasta algunas conclusiones sobre
los datos y KPI´s así como el uso de Power BI para el dashboard final.
 


## **Contexto del Proyecto**

Asumiendo el rol de Data Analist una empresa una empresa prestadora de servicios de telecomunicaciones nos encargo la realización de un análisis completo que permita reconocer el comportamiento de este sector a nivel nacional. Su principal actividad economica es la de brindar acceso a internet, pero también es importante considerar el comportamiento asociado al resto de los servicios de comunicación, con el fin de orientar a la empresa en brindar una buena calidad de sus servicios, identificar oportunidades de crecimiento y poder plantear soluciones personalizadas a sus posibles clientes. nos pide que realicemos un informe. 

Argentina ha experimentado un crecimiento constante en el acceso a Internet en los últimos años. En el segundo trimestre de 2023, el 88,4% de la población argentina tenía acceso a Internet, un aumento de 1,4% respecto al mismo trimestre del año anterior.

Este crecimiento se debe a una serie de factores, entre los que se incluyen la expansión de la cobertura de la red 4G, la disminución de los precios de los planes de Internet y la creciente penetración de los dispositivos móviles.

Según datos del Instituto Nacional de Estadística y Censos (INDEC), la región con mayor acceso a Internet en Argentina es la Patagonia, con una tasa del 91,8%. Le siguen Gran Buenos Aires, con un 88,4%, y la región de Cuyo, con un 89,2%.

Por consiguiente, este proyecto se enfocará específicamente en el analisis del **ACCESO A INTERNET** en Argentina, siendo que contamos con los datos de 



## **EDA (Análisis Exploratorio de Datos)**

- Calidad del dato:<br>

Se inició el EDA con una fase de preprocesamiento para limpiar el conjunto de datos. Esta etapa implicó familiarizarse con la **API** para realizar consultas, para ello tenemos disponible la [documentacion ](https://junar.github.io/docs/es/) la cual me permitio descargar los datasets. A su vez procedi al analisis de los mismos viendo cuales son los pertinentes y en base a sus datos comprobar si estos constan de valores nulos o faltantes, outliers, la corrección de formatos de datos y la unificación de tablas relevantes para un análisis más profundo. <br>



- Análisis de relaciones y patrones de los datos:<br>


Se exploraron diferentes variables presentes en el conjunto de datos, como la cantidad de accesos por tecnología, la distribución de servicios por provincia, la evolución de ingresos a lo largo de los años y otros factores relevantes dentro de la industria de las telecomunicaciones.<br>

Aqui podemos ver la **Distribucion de Accesos por cada 100 hogares por Provincia**

<p align='center'>
<img src ='src\imagen_distribuicones.png'>
<p>
Aqui podemos ver como La Provincia de Buenos Aires y Capital Federal son las que lideran la cantidad de accesos, a comparación del resto de las provincias. 


<p align='center'>
<img src ='src\evolucion.png' width="700" height="350">
<p>

Tambien podemos apreciar la tendencia claramente alcista de los accesos a internet por Hogar desde 2014 a 2022 en cantidad. <br>


<p align='center'>
<img src ='src\ingresos.png' width="700" height="350">
<p>

Tambien podemos ver como con el EDA esta tendencia alcista se ve reflejada en la cantidad de ingresos relacionados con el Acceso a Internet<br>

## **Enfoque del Storytelling del proyecto**

Tras analizar el EDA, se optó por centrar la narrativa del proyecto en los servicios de Internet, se presentará un KPI propuesto sobre como es la evolucion de accesos si cumplen o no la siguiente condicion trimestralmente:

`KPI de aumento en un 2% los accesos:` 
Aumentar en un 2% el acceso al servicio de internet para el próximo trimestre, cada 100 hogares, por provincia. <br>
La fórmula es la siguiente:<br>

 $`KPI = ((Nuevo acceso - Acceso actual) / Acceso actual) * 100`$
 
Donde:

- "Nuevo acceso" se refiere al número de hogares con acceso a Internet después del trimestre anterior.
- "Acceso actual" se refiere al número de hogares con acceso a Internet en el trimestre de referenica.
Es decir: <br>
Esta fórmula ayudará a calcular el KPI para medir el aumento en el acceso a Internet por cada 100 hogares en cada provincia para cualquier trimestre, ya sea para trimestres actuales siempre y cuando sean triemstres consecutivos.

**Ejemplo de uso:**

KPI = ((510 - 500) / 500) * 100 = 2%

Esto indicaría un aumento del 2% en el acceso a Internet en esa provincia para el próximo trimestre.


`KPI de aumento de los ingresos(2, 5 y 10%):`
Este KPI también cuenta con un filtro de porcentaje pero de incremento y hace la comparación de ingresos por trimestre, es decir se toma en cuenta dos trimestres y te da como resultado si conseguiste superar el aumento en un 2, 5 y 10% según lo seleccionado en el filtro. Por otro lado, este KPI puede funcionar tanto para Internet como para Telefonía ya que la estructura de ambos conjuntos de datos es muy similar.



## **Conclusión**

El análisis de datos aportados por ENACOM brinda un amplio panorama con múltiples variables, desde el rendimiento de accesos a Internet hasta la evolución de los ingresos a lo largo de los años. La visualización de datos fue una herramienta clave para comprender y presentar estos hallazgos. Por ejemplo, se identificaron cambios notables en los patrones de accesos a Internet, con un crecimiento exponencial en la conectividad móvil y un aumento significativo en la cobertura de fibra óptica.

El análisis permitió revelar tendencias de comportamiento y patrones de crecimiento, lo que resulta crucial para la toma de decisiones estratégicas y la mejora continua de los servicios de telecomunicaciones.

Sin embargo, es importante tener en cuenta que el entorno regulatorio y socioeconómico en el que opera la industria de las telecomunicaciones en Argentina también afecta el desarrollo de los servicios. Por ejemplo, la regulación de ENACOM, que obliga a una prestación básica universal y pone límites a las tarifas, puede influir en la oferta y la demanda de servicios. Además, la inflación, que es un factor clave en la economía argentina, puede afectar los precios de los servicios de telecomunicaciones.

Teniendo en cuenta estos factores, se puede concluir que el análisis de datos es una herramienta esencial para la industria de las telecomunicaciones en Argentina. Sin embargo, es importante realizar un análisis integral que tenga en cuenta el entorno regulatorio y socioeconómico en el que opera la industria.


## Fuentes de datos
**Obligatorio(Consigna del proyecto):**

- [Datasets principales](https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/) 

**Complementario:**
- [Datasets complementarios](https://datosabiertos.enacom.gob.ar/home)

**Información de Contacto:**
- [LinkedIn](https://www.linkedin.com/in/pablo-beti-714007265/)
- Correo electrónico: pablobeti@gmail.com

## Tecnologias utilizadas:
**Python - Power BI - Pandas - Seaborn** 

<body>
  <div class="logo-container">
    <img class="logo" src="src/Python-logo-notext.svg.png" width="100" height="100">
  </div>
    <div class="logo-container">
    <img class="logo" src="src/powerbi.jpg" width="150" height="100">
  </div>
  <div class="logo-container">
    <img class="logo" src="src/pandas.png" width="200" height="120">
  </div>
  <div class="logo-container">
    <img class="logo" src="src/seaborn.png" width="100" height="100">


</body>