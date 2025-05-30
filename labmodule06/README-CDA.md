# Constrained Device Application (Connected Devices)

## Lab Module 06

Be sure to implement all the PIOT-CDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
Mi implementación en este módulo se centra en el procesamiento de los datos de sensores y el envío de comandos a actuadores desde el dispositivo de borde (Constrained Device Application - CDA). Para ello, se crearon las clases correspondientes para simular sensores como temperatura, humedad y presión, y también un actuador para controlar la humidificación. Estos componentes se integraron en un gestor central llamado DeviceDataManager, el cual se encarga de recibir los datos generados por los sensores simulados, analizarlos y, si es necesario, enviar comandos a los actuadores para reaccionar ante determinadas condiciones ambientales (como una humedad baja). Además, el CDA puede comunicar datos hacia un servidor de borde (GDA) utilizando protocolos como MQTT.


How does your implementation work?
El funcionamiento de la implementación se basa en un ciclo continuo de generación de datos simulados por los sensores, los cuales son procesados en DeviceDataManager. Esta clase evalúa si las condiciones superan ciertos umbrales definidos (por ejemplo, humedad por debajo del 30%), y si es así, genera un comando para activar el actuador (humidificador). Además, los datos del sensor y los comandos pueden enviarse a través de MQTT al Gateway Device Application (GDA) para su almacenamiento o análisis. Todos los módulos y clases fueron organizados siguiendo la arquitectura del proyecto, asegurando modularidad y extensibilidad para usos posteriores en la nube u otras plataformas.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/iriaagullo/python-components/tree/labmodule06


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
