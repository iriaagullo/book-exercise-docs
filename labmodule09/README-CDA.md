# Constrained Device Application (Connected Devices)

## Lab Module 09

Be sure to implement all the PIOT-CDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

En esta implementación se incorporó la capacidad de recibir comandos de actuador por medio del protocolo MQTT en el CDA. Para ello, se configuró el MqttClientConnector para suscribirse al tópico correspondiente a los comandos emitidos por el GDA, y se integró la lógica necesaria en el DeviceDataManager para procesar estos mensajes entrantes. Cuando se recibe un mensaje, este se transforma desde su formato JSON a una instancia de ActuatorData, y se utiliza para ejecutar la acción correspondiente a través del manejador de actuadores (ActuatorAdapterManager).

How does your implementation work?

El CDA ahora también está preparado para enviar una respuesta de confirmación al GDA indicando si el comando fue procesado correctamente. Esto se realiza mediante la publicación de un mensaje MQTT en el tópico correspondiente a respuestas de actuadores. Este mecanismo de solicitud-respuesta entre GDA y CDA permite establecer un canal de comunicación bidireccional, facilitando el control remoto de dispositivos simulados desde la nube a través del GDA. Esta arquitectura simula de forma realista un escenario de IoT en el que el dispositivo final actúa como ejecutor de acciones controladas de forma centralizada.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/iriaagullo/python-components/tree/labmodule09



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

- CoapClientConnectorTest
- 
- 

EOF.
