# Laboratorio 4 instrumentación y Biosensores | Diseño y construcción de una incubadora neonatal a escala 

- Daniel Espinosa 5600778
- Samuel Velandia 5600777

# Introducción: 

Las incubadoras neonatales son dispositivos médicos diseñados para proporcionar un ambiente controlado que simula las condiciones del vientre materno, con el fin de garantizar la supervivencia y desarrollo adecuado del recién nacido.

Uno de los parámetros más críticos es la temperatura, la cual debe mantenerse aproximadamente en 37°C, ya que los neonatos, especialmente los prematuros, no tienen la capacidad de regular su temperatura corporal de manera eficiente.

El sistema de una incubadora generalmente incluye:

 - Un sistema de calefacción (resistencia eléctrica)
 - Un sistema de circulación de aire (ventilador)
Sensores para monitoreo (temperatura, peso, etc.)

Además, en condiciones extremas (como climas tropicales), también puede requerirse un sistema de enfriamiento.

<img width="750" height="750" alt="image" src="https://github.com/user-attachments/assets/dcae564c-785f-4159-a184-db8a17b74e56" />

Dónde esta práctica permite comprender la importancia del control de variables en sistemas biomédicos y las consecuencias de un mal funcionamiento.

# Objetivos : 

## Objetivo General : 

Analizar, diseñar y construir un prototipo funcional de incubadora neonatal a escala que permita comprender la importancia del control de variables biomédicas como la temperatura y el peso, así como su impacto en la estabilidad fisiológica y el adecuado desarrollo del recién nacido.

## Objetivo específico : 

- Identificar y comprender las principales partes que componen una incubadora neonatal, analizando la función de cada componente dentro del sistema y su relevancia en el cuidado del neonato.
  
- Diseñar y simular circuitos electrónicos que permitan el control de la temperatura mediante un sistema de lazo cerrado y la medición del peso utilizando sensores adecuados, aplicando conceptos de instrumentación biomédica.
  
- Construir un modelo a escala que integre los sistemas diseñados, evaluando su funcionamiento y verificando su capacidad para mantener condiciones controladas similares a las de una incubadora neonatal real.

# Materiales : 

- Multímetro digital
- Osciloscopio digital
- Fuente de voltaje DC
- Computador con internet
- Software de simulación de circuitos
- Protoboard
- Cable UTP
- Ventilador
- Reguladores LM317 y LM337
- Diodo 1N4007
- Transformador 502
- Fusible e interruptor
- Puente rectificador
- Termistor
- LEDs (3 unidades)
- Resistencias (1kΩ – 200kΩ)
- Capacitores (2200 µF)

  # Procedimiento:

  ## Parte A | Diseño y simulación :

En la primera etapa de la práctica, se realizó una revisión bibliográfica con el fin de identificar las principales partes que componen una incubadora neonatal, así como la función que cumple cada una dentro del sistema. Se analizaron elementos como la cámara de aislamiento, el sistema de calefacción, el ventilador, los sensores de temperatura y peso, y el sistema de control, comprendiendo cómo interactúan para mantener condiciones adecuadas para el neonato.

Posteriormente, se procedió al diseño y simulación de un sistema de control de temperatura en lazo cerrado. Para ello, se empleó un termistor como sensor encargado de medir la temperatura interna, cuya señal fue utilizada como retroalimentación para el sistema de control. Este sistema compara continuamente la temperatura medida con un rango de referencia establecido entre 36°C y 37.5°C, activando o desactivando un elemento calefactor según sea necesario. Adicionalmente, se incorporó un sistema de señalización mediante LEDs, donde un LED verde indica que la temperatura se encuentra dentro del rango adecuado, mientras que LEDs rojos alertan cuando la temperatura está por encima o por debajo de dicho rango.

<img width="1352" height="772" alt="image" src="https://github.com/user-attachments/assets/6e2f2b52-7ff2-43c7-a30d-1d4cebaa59b0" />


Finalmente, en esta parte se diseñó y simuló un circuito para la medición del peso, utilizando un sensor de fuerza que permite detectar variaciones de carga. La señal obtenida fue acondicionada para su correcta interpretación y posteriormente visualizada mediante un sistema de salida, como una pantalla LCD o displays de 7 segmentos, permitiendo así el monitoreo del peso del neonato de forma continua.

## Parte B | Construcción del prototipo : 

En la segunda etapa, se llevó a cabo la construcción física de un modelo de incubadora neonatal a escala, teniendo en cuenta las dimensiones aproximadas establecidas en la guía. Se utilizó un material transparente para la cubierta con el fin de garantizar la visibilidad del interior, así como un mecanismo que permitiera su apertura y cierre, facilitando el acceso al sistema interno.

A continuación, se implementó el sistema de control de temperatura previamente diseñado, integrando un ventilador para la circulación del aire y un elemento resistivo encargado de generar calor. Este sistema permitió mantener la temperatura dentro del rango establecido mediante un proceso de convección, distribuyendo el aire caliente de manera uniforme en el interior de la incubadora. Además, se instalaron los indicadores luminosos (LEDs) para mostrar en tiempo real el estado de la temperatura.

Posteriormente, se integró el sistema de medición de peso dentro de la estructura del prototipo, incorporando el sensor de fuerza y el sistema de visualización correspondiente. Esto permitió estimar el peso del neonato de manera práctica, simulando una de las funciones esenciales de las incubadoras reales.

Finalmente, se realizó una estimación del costo total del sistema desarrollado, considerando tanto el valor individual de cada componente como el costo global del prototipo. Asimismo, se efectuó una comparación general con incubadoras comerciales, teniendo en cuenta aspectos como funcionalidad, complejidad y costo.

## Parte C | Documentación : 

En la última etapa, se documentó todo el proceso desarrollado durante la práctica, describiendo de manera detallada cada uno de los pasos realizados en el diseño, simulación y construcción del sistema. Esta documentación se organizó siguiendo una estructura clara y coherente, facilitando su comprensión.

Adicionalmente, se creó un repositorio en la plataforma GitHub donde se recopiló toda la información del proyecto, incluyendo descripciones, diseños, simulaciones y evidencia del prototipo. Este repositorio permitió mantener un registro ordenado del trabajo realizado y fomentar el trabajo colaborativo entre los integrantes del grupo.

# Marco teórico : 

Las incubadoras neonatales son dispositivos biomédicos fundamentales en el cuidado de recién nacidos, especialmente en aquellos que presentan condiciones de prematurez o bajo peso al nacer. Su función principal es proporcionar un entorno controlado que simule las condiciones del útero materno, garantizando parámetros fisiológicos adecuados para la supervivencia y el desarrollo del neonato. Entre las variables más importantes que deben ser reguladas se encuentran la temperatura, la humedad, la oxigenación y el flujo de aire (Tran et al., 2014).

Uno de los aspectos más críticos en el funcionamiento de una incubadora neonatal es la termorregulación. Los recién nacidos, particularmente los prematuros, poseen una limitada capacidad para mantener su temperatura corporal debido a la inmadurez de su sistema nervioso y a la menor cantidad de tejido adiposo. Esto los hace altamente vulnerables tanto a la hipotermia como a la hipertermia, condiciones que pueden comprometer gravemente su estado de salud (Knobel-Dail, 2014). Por esta razón, las incubadoras deben mantener una temperatura estable alrededor de los 36°C a 37°C, rango considerado óptimo para el bienestar neonatal (EFCNI, 2018).

Desde el punto de vista de la ingeniería, el control de la temperatura en una incubadora se realiza mediante sistemas de control en lazo cerrado. En este tipo de sistemas, un sensor mide continuamente la variable de interés (temperatura), y esta información es retroalimentada a un controlador que compara el valor medido con un valor de referencia. En función de esta comparación, el sistema ajusta la acción de un actuador, como una resistencia calefactora, para mantener la variable dentro del rango deseado (Ogata, 2010). Este principio es ampliamente utilizado en sistemas biomédicos donde se requiere alta precisión y estabilidad.

<img width="582" height="386" alt="image" src="https://github.com/user-attachments/assets/5de38dff-e9ac-45fa-ac7f-124560dbb028" />


Para la medición de la temperatura, es común el uso de sensores como los termistores, los cuales presentan una variación de resistencia en función de la temperatura. Estos dispositivos son ampliamente utilizados debido a su bajo costo, alta sensibilidad y facilidad de integración en circuitos electrónicos (Webster, 2010). La señal generada por el sensor debe ser acondicionada adecuadamente para su procesamiento, lo que implica etapas de amplificación, filtrado y conversión analógica-digital.

Otro parámetro relevante en el monitoreo neonatal es el peso del recién nacido, el cual es un indicador clave del crecimiento y estado de salud. Para su medición se utilizan sensores de fuerza, como las galgas extensiométricas, que funcionan bajo el principio de deformación mecánica. Cuando se aplica una carga, el sensor experimenta una deformación que produce un cambio en su resistencia eléctrica, el cual puede ser medido y convertido en una señal proporcional al peso (Dally, Riley & McConnell, 1993).

Adicionalmente, las incubadoras incorporan sistemas de visualización e indicadores, como pantallas LCD o displays de 7 segmentos, que permiten mostrar información relevante al personal médico. También incluyen sistemas de alarma visual y auditiva que alertan cuando alguna variable se encuentra fuera de los rangos seguros, garantizando una respuesta rápida ante posibles fallos (Webster, 2010).

Desde una perspectiva más amplia, el desarrollo de incubadoras de bajo costo ha sido un tema de gran interés en la ingeniería biomédica, especialmente en países en desarrollo, donde el acceso a equipos médicos avanzados es limitado. Investigaciones han demostrado que es posible diseñar incubadoras funcionales con costos significativamente reducidos, manteniendo niveles aceptables de desempeño y seguridad (Tran et al., 2014).

<img width="466" height="466" alt="image" src="https://github.com/user-attachments/assets/264b25da-45c7-41fe-bd02-c3a78002d672" />

En conclusión, el diseño de una incubadora neonatal involucra la integración de conocimientos de electrónica, control automático y fisiología humana, permitiendo el desarrollo de sistemas capaces de garantizar condiciones óptimas para la vida neonatal. Este tipo de prácticas fortalece la comprensión de los estudiantes sobre la aplicación real de la instrumentación biomédica en la solución de problemas clínicos.
