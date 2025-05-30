# Gateway Device Application (Connected Devices)

## Lab Module 08

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

En esta implementación se añadió al Gateway Device Application (GDA) la capacidad de actuar como intermediario en la recepción de datos provenientes del CDA y su posterior transmisión a un servicio en la nube. Para ello, se incorporó la clase CloudClientConnector, la cual encapsula la lógica necesaria para transformar los datos recibidos en instancias de SensorData o SystemPerformanceData y enviarlos como JSON hacia el proveedor de servicios en la nube simulado. Se integró esta funcionalidad dentro del método handleUpstreamTransmission() del DeviceDataManager, el cual es invocado automáticamente cada vez que se recibe un nuevo mensaje desde el CDA mediante MQTT.

How does your implementation work?

Además, el GDA fue ajustado para almacenar los datos recibidos si la persistencia está habilitada, y analizar la información antes de reenviarla. La clase DeviceDataManager ahora maneja de manera efectiva mensajes de sensores, actuadores y rendimiento del sistema, permitiendo el flujo de información desde el CDA hasta la nube. De esta manera, el GDA funciona como un puente entre el borde de la red (edge) y el backend, cumpliendo el rol de agregador, procesador y retransmisor de datos IoT en un entorno simulado.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/iriaagullo/java-components/tree/labmodule08


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

- CoapClientToServerConnectorTest
- CoapServerGatewayTest
- 

EOF.
