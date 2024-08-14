**1.) ANÁLISIS DE LA EVOLUCIÓN DEL INTERNET EN L REPÚBLICA DE ARGENTINA**
 
**1.1) Descripción del Proyecto.**

Este proyecto tiene como finalidad describir la evolución y estado actual del servicio de internet en la república de Argentina, identificar tendencias y realizar una comparación con el resto de las telecomunicaciones. 

**1.2) Requisitos.**

Python versión: 3.7 o superior

MySQL version: 8.0.36

mysql-connector-python versión: 9.0.0

pandas versión: 2.1.4

numpy versión: 1.26.3

seaborn versión: 0.13.2

matplotlib versión: 3.8.3

scikit-learn version: sklearn preprocessing

PowerBI versión: 2.131.1203.0 64-bit

**1.3) Estructura del Proyecto.**

datasets: 

	1. Los datasets originales son: ‘Internet’, ‘Telefonia_movil’, ‘Television’, ‘telefonia_fija’. 
 
	2. ‘datos_limpios’ es el dataset ‘Internet’ después de las transformaciones. 
 
	3. ‘df_ingresos_accesos_100hab’ son los datasets de ‘Telefonia_movil’, ‘Television’, ‘telefonia_fija’ después de haber escogido la información de interés y haber realizado las transformaciones.	
 
	4. ‘df_gradienteinternet’ es un dataset calculado a partir del dataset ‘Internet’ para conocer el grado de cambio, en el tiempo, de algunas variables de interés. 
 
	5. 'df_kpi’, 'df_kpi2’ y 'df_kpi3’, son dataframes obtenidos a partir de internet para realizar el cálculo de los kpis del proyecto.
 
Notebook Segundo Proyecto: Notebook Jupyter donde se realiza carga de datos, transformación, visualizaciones, análisis y conclusiones del proyecto.

PowerBi Segundo Proyecto: presentación de los datos en un formato más atractivo.

**1.4) Uso y Ejecución.**

	1. Clonar el repositorio:  
	https://github.com/Jspadillahnr/Segundo_Proyecto_Integrado_Telecomunicaciones
 
	2. Instalar las librerías anteriormente nombradas.
 
	3. Abrir ‘Notebook Segundo Proyecto’ y correrlo todo. 
 
	4. Abrir ‘PowerBi Segundo Proyecto’, para poder revisar la presentación de los datos en un formato más llamativo.

**1.5) Datos y Fuentes.**

La fuente de los datos es ENACOM el cual es el Ente Nacional de Comunicaciones en Argentina. Este organismo se encarga de supervisar y controlar los servicios de telecomunicaciones, internet, radiodifusión y servicios postales en Argentina. 

**1.6) Metodología.**

A través del motor MySQL y mysql-connector-python se realiza la carga y transformación de los datos. Para la carga de datos se utiliza querys MySQL más Python para simplicar este proceso. Dentro de las transformaciones que podemos observar en el proyecto encontramos: transformación de las columnas a sus types correctos, identificación y tratamientos de nulos (‘null’y ‘nan’), identificación y tratamiento de outliers, identificación y eliminación de duplicados.  

Se emplean librerías de visualización para crear gráficos que permiten identificar patrones en los datos. Luego, esta información se transfiere a Power BI para presentar los resultados de manera más persuasiva y accesible.

**1.5) Análisis.**

*1.5.1) Gráfico de Tecnologías Por Años.*

![Distribución de tecnologías por año](https://github.com/user-attachments/assets/beee3f36-989d-4cd5-b2e5-d0814c1cfdea)

Lo primero que podemos notar en este gráfico es como han aumentado las personas con acceso a internet, a través de diferentes tecnologías, en al menos un 90% en los últimos diez años en la Argentina. Teniendo en cuenta que en estos años el porcentaje de crecimiento poblacional en este país ha sido de alrededor del 1%, podemos concluir que se ha hecho un esfuerzo enorme por aumentar el acceso de la población a internet; sin embargo, al compararlo con la población total de Argentina, el 75% de la población no tiene acceso a internet, por lo que aún hay un gran camino por recorrer.

Al revisar la suma de usuarios para todas las provincias a lo largo de los años, podemos notar que en el 2014 predominaban dos tecnologías por sobre el resto, el ADSL y el cablemódem, siendo el ADSL la tecnología con mayor porcentaje en el 2014; por otro lado, tecnologías como Wireless y Fibra Óptica para ese año tenían un mínimo porcentaje del mercado. Con el paso del tiempo, se puede ver como el cablemódem empieza a ganarle territorio al ADSL, hasta tal punto que pareciera que todos los usuarios que abandonaban la tecnología ADSL se empezaban a pasar al cablemódem, logrando este, alrededor del 2019, superar a la tecnología ADSL en termino de usuarios. Para entender esto debemos entrar un poco en la historia del internet. 

La primera infraestructura que se utilizó para transmitir datos fueron las líneas telefónicas, y allí por los años 80, el Dial-Up nos permitía andar, a duras a penas, a 56 kbps mientras no utilizáramos el teléfono. El teléfono, inventado en 1876 por Alexander Graham Bell, utilizaba las líneas telefónicas para transmitir la voz -una onda sonora que se propaga de manera continua en el tiempo- utilizando señales analógicas -señales electromagnéticos con amplitud y fase variables-. No fue hasta el año 1950 con la creación la modulación, una tecnología que permitía convertir señales digitales (1 y 0) provenientes de una computadora en señales analógicas, que se logró la conexión de dos computadores a distancia a través de las líneas telefónicas. El primer reto que trajo esto fue que la frecuencia utilizada para transmitir voz (300 Hz a 3400 Hz) era la misma para hacer la trasmisión de datos, de ahí que no se pudiera utilizar el internet y la línea telefónica al mismo tiempo. Con la evolución de las telecomunicaciones, se descubrió que se podían utilizar frecuencias más altas, la banda ancha, para la transmisión de datos y las más bajas para las de voz, surgiendo de esta manera la tecnología ASDL. Al utilizarse rangos de frecuencia más amplios, la velocidad aumento de una velocidad simétrica de 56 kps a una velocidad asimétrica de descarga entre 256 kbps y 24 Mbps y de subida entre 64 kbps y 1.4 Mbps. Un cambio radicalmente grande el generado por la modulación, cambio que no fue únicamente aprovechado por las empresas de telefonía ya que las empresas de televisión por cable se dieron cuenta que su red de cables coaxiales, especiales para la transmisión de señales de televisión (señales de alta frecuencia) podían ser una excelente opción para ofrecer transmisión de datos porque, al estar diseñada para altas frecuencias, permiten una mayor banda ancha y, por ende, logran un aumento en las velocidades entre 10 Mbps hasta 1 Gbps para descarga y 1 Mbps a 20 Mbps para subida. 

Principalmente es esta diferencia de velocidad la que atrajo muchas personas a realizar el cambio de tecnología ASDL a cablemódem. En Argentina las dos tecnologías fueron introducidas en el año 2000, y la tecnología ASDL empieza con una ventaja ya que la infraestructura para su funcionamiento ya existía, mientras que la evolución del cablemódem se fue dando a medida que la cobertura de la televisión por cable aumentaba en el territorio. 

Otro hito importante que podemos ver en el gráfico es la evolución de la fibra óptica. Antes del 2018, la participación de esta tecnología en el mercado, al igual que la Wireless, era bastante pequeña; sin embargo, de ahí en adelante esta empieza a ganar terreno de manera importante, tanto así que para el 2020 pareciera que el crecimiento del cablemódem se hubiera estancado y que ahora todos los nuevos usuarios, más los que siguieron dejando el ASDL, se pasaron a la fibra óptica. La evolución de esta tecnología se debe principalmente a que, a diferencia del ADSL y el cablemódem, esta tecnología no utilizaba infraestructura existente, por lo que, inicialmente, la inversión era más alta debido a la necesidad de desplegar nuevos cables de fibra y equipos; sin embargo, a medida que se ha aumentado la cobertura, el servicio se ha vuelto más asequible. A pesar de que, en cuanto a términos de velocidad, el cablemódem y la fibra óptica son similares; la fibra óptica, al utilizar pulsos de luz para transmitir los datos, es menos susceptible a interferencias electromagnéticas lo que produce menores deterioro en los cables y menores costos de mantenimiento y reparación, haciendo que esta tecnología se siga abriendo paso en el mercado.

*1.5.2) Gráfico de gradientes.*

![Gradiente de Cambio para Tecnologías y Acceso Cada 100 Hogares](https://github.com/user-attachments/assets/3b2bb582-89e4-4444-bff6-07e286a16a54)

Para las tecnologías este gráfico está construido de la siguiente manera:

〖Gradiente tecnología〗_i=(〖usuarios año nuevo〗_i- 〖usuarios año anterior〗_i)/(∑_i^n▒( 〖usuarios año nuevo〗_i- 〖usuarios año anterior〗_i))

Esta medida nos ayuda a dilucidar, cuantitativamente, como ha sido la evolución en el mercado de las diferentes tecnologías. Podemos ver que lo descrito anteriormente es acorde con esta nueva información: desde el 2016, donde la caída del ADSL es de un 4%, es decir, en vez de obtener nuevos usuarios, tuvo perdida de ellos y la perdida de estos, por como está calculado el gradiente, necesariamente es ganancia para otra tecnología, que, para este año, representa, en su mayoría, un aumento para el cablemódem que tiene un porcentaje del 97% de los nuevos usuarios de internet/traslados de otras tecnologías. Otras tecnologías, como Wireless y fibra óptica, abarcan, en este año, alrededor del 6% de los nuevos usuarios. 

Esta tendencia continua hasta el 2018, donde la pérdida de usuarios ADSL sigue en aumento, siendo estas pérdidas, prioritariamente, nuevos usuarios para el cablemódem, aunque se debe hacer una mención especial para la tecnología Wireless, que en el gráfico de barras se veía menos significativa, pero que, sin embargo, su porcentaje, para el 2018, era del 18%. De este año para adelante la tragedia para el ADSL es inminente, con una pérdida de usuarios de un 83% en el 2019 y de un máximo de 270% en el 2020, el año de la pandemia, lo que podría significar que mucha gente decidió buscar mejores velocidades de internet y, por ende, migrar a otras tecnologías debido a la necesidad de trabajar en casa. En esta misma época que empieza el surgimiento de la fibra óptica, donde el 2019 se queda con el 63% de los nuevos usuarios/traslados y con un máximo de 189% en el 2020, superando al cablemódem. Para esto mismos años, el aumento del cablemódem es de 101% y 156%, por lo que, en resumidas cuentas, en estos dos años la pérdida de usuarios del ASDL son traslados al cablemódem o la fibra óptica.

En el 2021, la velocidad de pérdida de usuarios del cablemódem se reduce a un 54%, y podemos seguir viendo un reparto relativamente equitativo entre el cablemódem y la fibra óptica, con porcentajes de 71% y 56% respectivamente, sin embargo, después de este año el porcentaje de nuevos usuarios para el cablemódem cae drásticamente, con un porcentaje del 31% en el 2022 y con una pérdida del 3% para el 2023. Esto significa que, en estos últimos años, la mayoría de pérdida de usuarios del ADLS se trasladaron a la fibra óptica y que, incluso, para el 2023, usuarios de ADLS y Cablemódem se trasladaron a la fibra óptica. Los porcentajes de ganancia de usuarios para la fibra óptica en los últimos años son de 115% y 206%
Ahora que ya hablamos de los nuevos usuarios y traslados entre tecnologías, podemos ver otras dos variables importantes en este gráfico: el gradiente de los accesos por cada 100 habitantes y el de los ingresos. Es interesante notar que la media del aumento en el porcentaje de los accesos por cada 100 habitantes ronda el siete por ciento, mientras que los ingresos tienen una media de aumento del 40%. En un comienzo esto podría parecer contraintuitivo ya que lo lógico sería pensar que los dos deberían aumentar equitativamente. Esta discrepancia se puede entender debido a que el ADSL suele tener planes más baratos debido a que esta tecnología es menos costosa de mantener, además de que los costos de infraestructura ya están amortizados en gran medida. Al haber un traslado masivo de esta tecnología a tecnologías con planes más costosos como el cablemódem y la fibra óptica, esto, claramente, afecta los ingresos percibidos.

*1.5.3) Gráfico Tecnologías por Provincias.*

![Distribución de tecnologías por provincia](https://github.com/user-attachments/assets/4c825e20-9daf-46e3-a756-e357c2e7d717)

En nuestro gráfico de tecnologías, estamos viendo un comportamiento promedio de todas las provincias, pero, teniendo en cuenta que la provincia de Buenos Aires ocupa casi el 50% de la población de Argentina, esta gráfica puede ser una buena aproximación para esa provincia, pero, y el resto ¿sigue este comportamiento? 
Provincias como Chaco, Córdoba, Corrientes, Misiones, Salta, Santiago del Estero, Santa fe, Entre Ríos, La Rioja y Jujuy tienen un comportamiento similar con la provincia de Buenos Aires en cuanto a la evolución de las tecnologías a lo largo del tiempo, con algunas variaciones en los tiempos donde suceden los hitos y la participación de la tecnología Wireless y Otras. 
La Capital federal y Tierra del Fuego tiene una configuración peculiar poque si bien se nota el descenso de del ADSL, en ninguna de los dos existe un surgimiento de la fibra óptica. En el caso de Tierra de Fuego esto puede tener sentido, ya que es la provincia con menos habitantes de Argentina, y puede que los tendidas de líneas de fibra óptica aún no sean una realidad allí, pero en el caso de la capital resulta un poco extraño que no haya pocos servicios de fibra óptica disponible. 
Provincias como Formosa, la Pampa, Rio Negro, Neuquén, San Juan, Chubut y Santa Cruz tienen una particularidad y es que, a pesar de seguir con las tendencias de migración de tecnologías de la provincia de Buenos Aires, en estas provincias existen una fuerte influencia de las tecnologías un poco menos tradicionales, como Wireless y Otras.
Catamarca, Mendoza y Tucumán, tienen una disposición bastante curiosa, ya que más se ve una predominancia del ADSL hasta años después de la media de los anteriores y la primera ola de migración de ADLS a cablemódem está muy por debajo de las otras provincias, pero sí se ve un efecto más acentuado a la migración de la fibra óptica en los últimos años.
El caso de San Luis es el más extraño de todos, con una dominancia casi en una totalidad del Wireless y Otros como las tecnologías para proveer internet; sin embargo, en los últimos años se empieza a notar una pequeña inserción del cablemódem y la fibra óptica. Esto se debe a que, debido a la configuración de su territorio con montañas y zonas rurales extensas, representa un desafío para el tendido de los cables, por lo que el Wireless representa la mejor opción para el acceso a internet en esta provincia. 

*1.5.4) Gráfico Velocidades por Año.*

![distribucion de velocidades de internet por año](https://github.com/user-attachments/assets/80b6b5d4-ef41-4a4e-a607-09e577c665f3)

Habiendo hablado de las diferentes tecnologías de internet a lo largo de los últimos años en Argentina, esto nos da pie para entender cómo han variado las velocidades de internet en este periodo.

En el año 2014, prácticamente todas las velocidades de internet se encontraban entre 1 Mbps - 6 Mbps, velocidades fácilmente alcanzables por las tecnologías de banda ancha disponibles en la época: el cablemódem y ADSL, tecnologías que ocupaban casi la totalidad del mercado para ese año. Con el paso de los años vemos una transición considerable a velocidades entre 6 Mbps a 20 Mbps, principalmente de 6 Mbps a 10 Mbps, posiblemente por actualizaciones que permitían una mejor velocidad en las dos tecnologías y, para el 2018, vemos que el mercado esta dividido en dos por velocidades de 1 Mbps a 6 Mbps y 1 mayores 6 Mbps repartidas por igual; en este último mayor el porcentaje de 6 Mbps a 20 Mbps, aunque con una ligera participación de más de 30 Mbps que se podría atribuir al comienzo de la ascensión de la fibra óptica. Del 2018 en adelante vemos un ingreso bastante considerable de velocidades de 20 Mbps a 30 Mbps y más de 30 Mbps, especialmente de la última, y un considerable bajonazo en las velocidades de 1 Mbps a 6 Mbps. Teniendo en cuenta que es este mismo año donde se empieza a ver una caída abrupta en los usuarios del ADSL, podemos considerar que este cambio se debe principalmente a usuarios dejando esta tecnología para buscar rangos de velocidad mucho más altos con tecnologías como el cablemódem y la fibra óptica. 

Indudablemente, como lo vemos en la gráfica de velocidad media en el territorio, esta ha aumentado un increíble 1300%, lo que muestra una evolución en las tecnologías e infraestructura de estas en el país. Podemos ver que, en general, la velocidad promedio tiene un incremento estable, pero en el 2022 tiene un crecimiento muy grande que justo está ubicado en fechas similares en lo que empieza a hacer el descenso del cablemódem con respecto a la fibra óptica y esto tiene sentido ya que la fibra óptica es superior cuando se trata de proveer altas velocidades de internet. Es más eficiente, tiene una mayor capacidad de transmisión, mantiene mejor la calidad de la señal sobre largas distancias, y es más resistente a las interferencias.  

*1.5.5) Gráfico Velocidades por Provincia.*

![Distribucion de velocidades de internet por provincia](https://github.com/user-attachments/assets/0543bb30-b417-45a9-a11a-03ee0520069a)

La distribución de los grupos que vimos en las tecnologías por provincias es similar al que podemos encontrar en las velocidades por provincias. 
A diferencia de nuestro análisis respecto a las tecnologías de las provincias, en cuanto a velocidad podemos formar un grupo más grande y generalizado. Todas las provincias, a excepción de la Capital Federal y San Luis, tienen comportamiento similar con la provincia de Buenos Aires, con variaciones en los tiempos donde suceden los hitos y la participación de las diferentes velocidades. 

La razón de poder unir a la mayoría de las provincias en un sólo grupo es porque es porque, como mencionamos en el análisis de las tecnologías por provincia, había unas que sólo se diferenciaban por un mayor desarrollo de la tecnología Wireless y la fibra óptica. Estas tecnologías tienen velocidades superiores a los 20 Mbps haciendo que, a pesar de ser diferentes tecnologías, la velocidad es similar.

Para las provincias Salta, Entre Ríos, Tierra de Fuego y Santiago de Estero, podemos ver que, en los últimos años, a diferencia de las otras provincias, la participación de velocidades de 20 Mbps a 30 Mbps es una parte considerable del mercado, siendo que, en el caso de Tierra de Fuego y Santiago de Estero, la participación de 30 Mbps o más es bastante pequeña comparada con esta. 

De las provincias La Rioja, Formosa, la Pampa, Río Negro, San Juan, Chubut, Santa Cruz podemos ver que, a pesar de seguir el patrón, el desarrollo de este empieza tardíamente en comparación con las otras provincias de este grupo.

El caso de la Capital Federal es bastante diferente. Para el 2020 la velocidad es, prácticamente 30 Mbps o más. Como vimos en el análisis de tecnología y provincias, desde el 2014 ya la mayoría del servicio era proveído por el cablemódem, lo cual le da sentido que el desarrollo de esta provincia haya sido más rápido que el del resto.
El caso San Luis, en el cual la tecnología Wireless manda la parada, debemos tener en cuenta que la evolución ha sido principalmente de 20 Mbps a 30 Mbps. Teniendo en cuenta que las velocidades del Wireless varían entre 20 Mbps a 50 Mbps, es decir son menores en comparación a tecnologías como el cablemódem y la fibra óptica, este comportamiento tiene sentido.

*1.5.6) Internet vs Otras Telecomunicaciones.*

1.5.6.1) Accesos por cada 100 habitantes.

Lo que podemos ver a primera vista es la abrupta caída del acceso de la telefonía móvil, que cae de un 44% a un 21%, teniendo un mínimo en el 2020 de 16%; la telefonía fija también ha sufrido un descenso del 23% al 16%. Por otra parte, tanto el internet como la TV por subscripción, o cable, han tenido un aumento, de 10% a 20% y de 14% a 17%, respectivamente. En el caso de la TV satelital, ha tenido una caída del 6% al 4%.

Para entender un poco la caída tan abrupta de la telefonía móvil y la caída, menos áspera de la telefonía fija, debemos revisar un poco el contexto económico del país. Desde el 2014, la media de la inflación ha sido del 70%, una situación difícil que afecta significativamente el poder adquisitivo de los ciudadanos. En un entorno marcado por una economía difícil, además teniendo en cuenta que ahora existen aplicaciones VoIP que eliminan las necesidades de llamadas con una línea normal, es muy posible que los usuarios hayan decidido priorizar el internet sobre los servicios de telefonía.

En el caso de la televisión por cable, se considera que su aumento está totalmente ligada a los aumentos de accesos en el internet. Debemos recordar que el cablemódem, una de las tecnologías más importantes para prestar el servicio de internet, utiliza las líneas de la televisión por cable para hacer la transmisión de datos. Debido a que las compañías que proveen televisión por cable vendes paquetes completos, es muy probable que una parte de la población que haya buscado servicio de internet a través de esta tecnología, por defecto, haya también incluido un paquete de televisión por cable.

1.5.6.2) Ingresos.

La tendencia que siguen los ingresos es proporcional a la cantidad de accesos de la tecnología, a excepción de la telefonía móvil; entre más accesos, más ingresos.
Cómo se había mencionado antes, a pesar de ser contraintuitivo que, en el caso de la telefonía móvil, se disminuyan los accesos e igual haya un aumento en los ingresos, esto se puede deber al incremento en el uso de planes de datos para internet, nivelando un poco la pérdida de usuarios. 
En el caso de la telefonía fija, esta al ser la tecnología más económica, es normal que sea la de menores ingresos. A pesar de que esta también sufre de una perdida de clientes a lo largo de los años, su caída no es tan grande como la de la telefonía móvil, por lo que podemos suponer que ajustes en los costos de los planes mantienen los ingresos estables. 
Vemos que tenemos un repunte en los ingresos de todas las tecnologías desde el 2022. Esto se pude deber principalmente a que la inflación paso del 50% al 90% en el 2022; para el 2023 la inflación era del 211%; esto, claramente, afecta el ingreso nominal de las telecomunicaciones sin que se vea afectado realmente el consumo. 

**1.7) Conclusiones.**

	1. A pesar de que ha habido un 90% de crecimiento en los accesos de internet, aún el 75% de la población no tiene acceso a él.
 
	2. El descubrimiento de nuevas tecnologías ha permitido el aumento de la banda ancha, y por ende la velocidad del internet. Desde 2014, las velocidades de internet en Argentina 	han aumentado significativamente, con una transición de 1-6 Mbps a más de 30 Mbps, impulsada por la adopción de tecnologías como el cablemódem y la fibra óptica.
 
	3. Las nuevas tecnologías han causado migraciones de un servicio a otro. En el caso particular de Argentina, hay una migración alta de ADSL a cablemódem, Wireless y fibra óptica.
	Aunque el porcentaje de accesos a internet por cada 100 habitantes ha aumentado en promedio un 7%, los ingresos han crecido significativamente más, con una media del 40%. Esta 	discrepancia se atribuye al cambio de usuarios de ADSL, una tecnología más económica, hacia tecnologías más costosas como el cablemódem y la fibra óptica, lo que ha incrementado 	los ingresos de manera
 
	4. El comportamiento de las diferentes provincias, tanto en tecnologías como en velocidad es muy general al del país, con variaciones entre las fechas que suceden los hitos sin 	embargo, existen provincias como San Luis con un comportamiento totalmente atípico. 
 
	5. Los accesos a la telefonía móvil y fija han disminuido significativamente, debido a la inflación y al uso de aplicaciones VoIP que reemplazan llamadas tradicionales.
	Los accesos a internet y TV por cable han aumentado, probablemente porque muchos usuarios adquirieron ambos servicios en paquetes combinados ofrecidos por proveedores de 		cablemódem.
 
	6. Los ingresos de las telecomunicaciones han seguido siendo estables o han aumentado, impulsados por el aumento en el uso de datos móviles y los ajustes de precios en un 		contexto de alta inflación.
