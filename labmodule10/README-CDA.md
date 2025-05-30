# Constrained Device Application (Connected Devices)

## Lab Module 10

Be sure to implement all the PIOT-CDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Esta implementación en el CDA permite manejar los comandos de actuador recibidos desde el GDA y proporcionar respuestas de manera automática. Se agregó soporte en la clase DeviceDataManager para procesar tanto comandos de actuadores como mensajes de respuesta, y se mejoró la conexión MQTT para que se puedan publicar y suscribirse a los tópicos necesarios. Cuando el CDA recibe un comando, este es pasado al ActuatorAdapterManager, que activa o desactiva el actuador simulado dependiendo del tipo de comando recibido.

How does your implementation work?

Además, tras procesar el comando, el CDA genera una respuesta con el resultado de la ejecución (éxito o error) y la envía de vuelta al GDA usando el mismo canal MQTT. Esto asegura que el GDA tenga visibilidad del estado del actuador en el CDA. También se realizaron ajustes para garantizar que los datos se registren correctamente, y que el CDA actúe como un dispositivo de borde capaz de recibir, ejecutar y reportar comandos de manera eficiente, robusta y segura dentro de un entorno IoT simulado.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/iriaagullo/python-components/tree/labmodule10


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
- DeviceDataManagerCallbackTest
- DeviceDataManagerIntegrationTest

### Results

Hay algún test que no estoy segura de que esté bien del todo porque me dejó de funcionar SenseHAT sin razón aparente.

EOF.
