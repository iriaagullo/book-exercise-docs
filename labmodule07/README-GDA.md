# Gateway Device Application (Connected Devices)

## Lab Module 07

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

En esta implementación se añadió la capacidad de comunicación entre el dispositivo CDA y el servidor GDA a través de MQTT, estableciendo una conexión pub/sub robusta y flexible. Para ello, se configuró y utilizó un cliente MQTT (MqttClientConnector) que permite publicar mensajes desde el CDA hacia el GDA y suscribirse a diferentes topics definidos por recursos (sensor, actuador, rendimiento del sistema, etc.). Se configuraron los tópicos adecuados en el archivo config.props, y se verificó el correcto envío y recepción de datos en formato JSON, utilizando la clase DataUtil para serialización y deserialización.

How does your implementation work?

El flujo de datos comienza con la generación de información por los sensores simulados (temperatura, humedad y presión). Esta información es procesada por DeviceDataManager, quien utiliza el cliente MQTT para enviar estos datos al GDA. Además, el CDA también se suscribe a los comandos de actuadores provenientes del GDA, permitiendo simular una comunicación bidireccional. En resumen, esta implementación permite que el CDA actúe tanto como productor de datos hacia el GDA como consumidor de comandos, consolidando un entorno de comunicación completo basado en MQTT.


### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/iriaagullo/java-components/tree/labmodule07


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

- MqttClientConnectorTest
- MqttClientControlPacketTest
- 

EOF.
