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

Finalmente, en esta parte se diseñó y simuló un circuito para la medición del peso, utilizando un sensor de fuerza que permite detectar variaciones de carga. La señal obtenida fue acondicionada para su correcta interpretación y posteriormente visualizada mediante un sistema de salida, como una pantalla LCD o displays de 7 segmentos, permitiendo así el monitoreo del peso del neonato de forma continua.

## Parte B | Construcción del prototipo : 

En la segunda etapa, se llevó a cabo la construcción física de un modelo de incubadora neonatal a escala, teniendo en cuenta las dimensiones aproximadas establecidas en la guía. Se utilizó un material transparente para la cubierta con el fin de garantizar la visibilidad del interior, así como un mecanismo que permitiera su apertura y cierre, facilitando el acceso al sistema interno.

A continuación, se implementó el sistema de control de temperatura previamente diseñado, integrando un ventilador para la circulación del aire y un elemento resistivo encargado de generar calor. Este sistema permitió mantener la temperatura dentro del rango establecido mediante un proceso de convección, distribuyendo el aire caliente de manera uniforme en el interior de la incubadora. Además, se instalaron los indicadores luminosos (LEDs) para mostrar en tiempo real el estado de la temperatura.

Posteriormente, se integró el sistema de medición de peso dentro de la estructura del prototipo, incorporando el sensor de fuerza y el sistema de visualización correspondiente. Esto permitió estimar el peso del neonato de manera práctica, simulando una de las funciones esenciales de las incubadoras reales.

Finalmente, se realizó una estimación del costo total del sistema desarrollado, considerando tanto el valor individual de cada componente como el costo global del prototipo. Asimismo, se efectuó una comparación general con incubadoras comerciales, teniendo en cuenta aspectos como funcionalidad, complejidad y costo.

## Parte C | Documentación : 

En la última etapa, se documentó todo el proceso desarrollado durante la práctica, describiendo de manera detallada cada uno de los pasos realizados en el diseño, simulación y construcción del sistema. Esta documentación se organizó siguiendo una estructura clara y coherente, facilitando su comprensión.

Adicionalmente, se creó un repositorio en la plataforma GitHub donde se recopiló toda la información del proyecto, incluyendo descripciones, diseños, simulaciones y evidencia del prototipo. Este repositorio permitió mantener un registro ordenado del trabajo realizado y fomentar el trabajo colaborativo entre los integrantes del grupo.
