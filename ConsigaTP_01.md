# Trabajo práctico TopRad 2024

<ins> Una práctica que se recomienda es crear un proyecto de trabajo para este curso si se está trabajando con spyder</ins>

## Ejercicio 0 - Antes de empezar
1. Implemente las siguientes funciones (para un año no bisiesto) en función del dı́a ordinal y una ubicación especificada por su latitud (φ) y longitud (ψ):
    -Factor de corrección orbital, Fn .
    -Declinación solar, δ.
    -Áltura solar máxima, αsmax y ángulo cenital mı́nimo, θzmin .
    -Ángulo horario de puesta del Sol, ωs .
    -Azimut solar a la puesta del Sol, γs .
    -Ecuación del tiempo, E, en minutos.
    -Cantidad de horas diurnas, en horas y fracción (tiempo estándar).
    -Irradiación diaria en el Tope de la atmósfera (TOA) en incidencia normal, en MJ/m2.
    -Irradiación diaria TOA sobre un plano horizontal, en MJ/m2 .


2. Implemente las siguientes funciones, para un dı́a ordinal y ubicación dada, en función del ángulo horario asociado a cada minuto del dı́a (tome las 24 horas del dı́a y establezca las modificaciones necesarias en la serie temporal para una correcta visualización nocturna).

3. Calcule la serie temporal del ángulo cenital (θz ), la altura solar (αs ) y el ángulo azimutal (γs ). Grafique estas funciones para dı́as próximos a ambos solsticios y para uno de los equinoccios en función del ángulo horario y la hora del dı́a.

4. Grafique la trayectoria solar de ese dı́a en un diagrama (γs , αs ).

5. ¿A qué hora del dı́a en UTC-3 ocurre el mediodı́a solar exactamente?

## Ejercicio 1 - Irradiación TOA y cantidades básicas

- Visualice gráficamente las funciones implementadas previamente (Ejercicio 0 parte (1)) variando
el dı́a del año entre 1 y 365 para Salta (φ = −24.72◦ , ψ = −65.4◦ ).
- ¿Cuáles son los dı́as más
corto y largo del año?
- ¿En qué dı́as del año se obtiene la máxima irradiación diaria TOA sobre
plano horizontal?
- Compare cuantitativamente con la máxima irradiación diaria TOA sobre plano
horizontal calculada para el mismo meridiano, pero en el hemisferio norte (φ = -24◦ , ψ = −65.7◦ ).


## Ejercicio 2 - Duración del dı́a solar
El ángulo horario ω define el Tiempo Solar Aparente, Ts . La duración del dı́a solar para un
observador dado en la superficie terrestre, puede definirse como el intervalo de tiempo (en horas y
fracción) entre dos cruces sucesivos del Sol por el meridiano del observador.

1. Para Salta (φ = −24.75◦ , ψ = −64.7◦ ) determinar (en horas y fracción) la duración del dı́a
solar, para cada dı́a de un año no bisiesto. Graficar y comentar el resultado. ¿Cuál es la relación
de la duración del dı́a solar con la ecuacion de tiempo?
2. ¿En qué dı́as del año el dı́a solar dura exactamente 24 horas?


## Ejercicio 3 - Medidas y Modelos de Cielo Claro

Vamos a trabajar con un conjunto de datos que fueron proporcionados para la estación Goodwin Creek (GWN) de la red SURFRAD (https://gml.noaa.gov/grad/surfrad/index.html) de EEUU. Se proporciona un archivo CSV (Comma Separated Values) para esta estación. La estación de medida se encuentra en Latitud = +34.2547. Longitud = -89.8729. Altura = 98 m s.n.m.

***consulte el contenido Clase_01/Acceso Ficheros del material del curso***


_Al trabjar con la serie de datos usted puede escoger el archivo con el formato de etiqueta temporal que le sea más conveniente._

Realice los siguientes gráficos y analícelos:
1. Serie temporal de la medida de GHI y su correspondiente irradiancia extraterrestre.
2. Serie temporal de la medida de GHI y la estimación de cielo claro del modelo McClear (columna
GHIcsk incluida en el archivo de datos).
3. Serie temporal del índice de claridad y del índice de cielo claro.
4. Gráficos de la GHI, del índice de cielo claro y del índice de claridad vs el coseno del ángulo
cenital en el eje x.

**Interprete cada uno de los gŕaficos**

