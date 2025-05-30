# Gateway Device Application (Connected Devices)

## Lab Module 10

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Esta implementación en el GDA permite recibir datos de sensores desde el CDA, analizarlos y generar comandos de actuador en función de ciertos umbrales definidos en la configuración. En concreto, el DeviceDataManager del GDA analiza los datos de humedad recibidos y, si están fuera de los valores aceptables, genera comandos para activar o desactivar el humidificador. Estos comandos son enviados al CDA mediante MQTT. Además, se ha implementado la lógica para manejar las respuestas a estos comandos, que llegan desde el CDA confirmando si el actuador ejecutó correctamente la orden.

How does your implementation work?

El GDA también suscribe los tópicos relevantes al iniciarse y maneja tanto los mensajes de sensores como los de rendimiento del sistema. Se asegura de que los mensajes sean almacenados (si el cliente de persistencia está habilitado) y que sean reenviados al servicio en la nube (si el cliente cloud está activado). Esta arquitectura refuerza el rol del GDA como un nodo de control inteligente, capaz de tomar decisiones en base a datos en tiempo real y mantener una comunicación bidireccional fluida con el CDA y otros servicios conectados.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/iriaagullo/java-components/tree/labmodule10



### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- 
- 
- 

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- MqttClientPerformanceTest
- CoapClientPerformanceTest
- MqttClientConnectorTest
- DeviceDataManagerSimpleCdaActuationTest

EOF.
