# Shield iBlock

Shield para Arduino Uno R3 (y tarjetas que comparten las mismas dimensiones) que permite conectar módulos y accesorios compatibles con el sistema iBlock desarrollado por Geek Factory.

Este shield "exporta" los puertos de la tarjeta Arduino Uno a cables planos de 10 hilos que pueden usarse para interconectar con otros módulos o el protoboard.

El sistema iBlock esta diseñado para usarse durante el aprendizaje de sistemas digitales programables o para desarrollar aplicaciones finales.

![Shield ioBlock](https://raw.githubusercontent.com/geekfactory/shield-iblock/master/extras/shield-iblock.JPG)

## Sistema iBlock

Se trata de una solución de conectividad diseñada para facilitar la reutilización de hardware en prototipos y sistemas realizados para producción. Esta basada en el uso de conectores [IDC (Insulation Displacement Connector)](https://en.wikipedia.org/wiki/Insulation-displacement_connector) y cable plano.

Principalmente se contempla el uso de conectores de 10 pines que permoiten llevar 8 bits o pines de I/O de propósito general y además la tierra y el voltaje de alimentación.

En este sistema cada uno de los módulos se diseñan con una distribución de pines conocida, de forma que sea posible intercambiar y reutilizar el hardware según las necesidades del proyecto.

La distribución de pines en el conector IDC-10 es la siguiente:

1. D0
2. D1
3. D2
4. D3
5. D4
6. D5
7. D6
8. D7
9. GND
10. V+ (3.3 o 5 volts)

Como el arduino Uno dispone de más puertos digitales, se continua en otro conector:

1. D8
2. D9
3. D10
4. D11
5. D12
6. D13
7. NC (sin conexión)
8. NC (sin conexión)
9. GND
10. V+ (3.3 o 5 volts)

La distribución es similar para los pines analógicos de la tarjeta.

## Periféricos y características

* 3 conectores IDC-10 que exponen todos los puertos digitales y analógicos de la tarjeta arduino
	* DIGITAL1 - Expone los pines del 0 al 7 digitales
	* DIGITAL2 - Expone los pines del 8 al 13 digitales
	* ANALOG1 - Expone los pines A0 al A5 analógicos
* 20 conectores tipo servo que brindan acceso a la alimentación y a todas las señales (D0 - D13 y A0 - A5)
* Diseño apilable que permite colocar otros shields o accesorios arriba de esta placa, incluso el conector SPI (ISP) se replica a otros shields
* Se utilizan conectores IDC-10 en angulo que permite la conexión del cable plano cuando hay otro shield colocado encima
* Selección de voltaje de alimentación (3.3 volts o 5 volts) en cada uno de los conectores IDC-10 mediante interruptores
* Conector Nanobus que permite expandir la funcionalidad del shield con otros módulos desarrollados para este estándar
* Dimensiones del PCB: 76.2 mm x 53.34mm (3 x 2.1 pulgadas)

## Contenido del repositorio

1. __root__ - Archivos fuente de EAGLE para esta placa
2. __/documents__ - Documentación adicional, hojas de datos de componentes e instrucciones de ensamble
3. __/production__ - Histórico de gerbers enviados a producción
4. __/extras__ - Dibujos técnicos, imagehes, hardware de montaje adicional y diseños de accesorios relacionados
4. __/firmware__ - Si existe el firmware de prueba o definitivo de esta placa

## Licencia de uso

**Este proyecto se publica como hardware de codigo abierto. Favor de leer detenidamente el archivo license.md para información detallada de la licencia.**

**Reconocimiento-NoComercial-CompartirIgual 4.0 Internacional (CC BY-NC-SA 4.0)**

Esto es un resumen inteligible para humanos (y no un sustituto) de la licencia.

Usted es libre de:

* __Compartir__ — copiar y redistribuir el material en cualquier medio o formato
* __Adaptar__ — remezclar, transformar y crear a partir del material

El licenciador no puede revocar estas libertades mientras cumpla con los términos de la licencia.

Bajo las condiciones siguientes:

* __Reconocimiento__ — Debe reconocer adecuadamente la autoría, proporcionar un enlace a la licencia e indicar si se han realizado cambios. Puede hacerlo de cualquier manera razonable, pero no de una manera que sugiera que tiene el apoyo del licenciador o lo recibe por el uso que hace.

* __NoComercial__ — No puede utilizar el material para una finalidad comercial.

* __CompartirIgual__ — Si remezcla, transforma o crea a partir del material, deberá difundir sus contribuciones bajo la misma licencia que el original.

No hay restricciones adicionales — No puede aplicar términos legales o medidas tecnológicas que legalmente restrinjan realizar aquello que la licencia permite.

## Versiones del Hardware

* 1.0 - Versión inicial