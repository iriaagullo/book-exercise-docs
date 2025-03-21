# Gateway Device Application (Connected Devices)

## Lab Module 05

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

En la GDA, se han implementado funcionalidades similares a las de la CDA para la serialización y deserialización de datos en formato JSON. Además, se ha añadido soporte para la persistencia de datos utilizando la interfaz IPersistenceClient, permitiendo el almacenamiento y recuperación de datos en una base de datos de series temporales.

How does your implementation work?

La clase DataUtil en la GDA maneja la conversión de objetos de datos a y desde JSON. La implementación de la interfaz IPersistenceClient permite que la GDA interactúe con una base de datos de series temporales, facilitando la gestión de datos históricos y la comunicación eficiente entre la CDA y la GDA.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/iriaagullo/java-components/tree/labmodule05

Rama: labmodule05

### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest
- DataUtilTest
- PersistenceClientTest
- GatewayDataManagerTest

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- GatewayDataIntegrationTest
- CloudConnectivityTest
- DeviceCommunicationTest

EOF.
