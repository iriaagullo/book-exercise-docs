# Gateway Device Application (Connected Devices)

## Lab Module 11

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Esta implementación en el GDA se enfoca en agregar soporte para la persistencia de datos provenientes del CDA. Para ello, se integró una instancia de IPersistenceClient en la clase DeviceDataManager, que se activa si el parámetro de configuración correspondiente está habilitado. Cuando se recibe un mensaje de sensor (SensorData), el GDA almacena esta información usando el método storeData, asegurando que los datos sean guardados de forma local para su posterior análisis o consulta.

How does your implementation work?

El enfoque seguido consiste en detectar la llegada de nuevos datos desde el CDA, y antes de cualquier otro procesamiento, validar que el cliente de persistencia esté habilitado y disponible. Si lo está, los datos se guardan utilizando una calidad de servicio (QoS) estándar. Esta mejora permite al GDA actuar como un nodo intermedio robusto, que no solo enruta información, sino que también la conserva localmente, incrementando la confiabilidad del sistema en entornos con conectividad intermitente o para auditorías locales.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL:  https://github.com/iriaagullo/java-components/tree/labmodule11


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
- CloudClientConnectorTest
- 

EOF.
