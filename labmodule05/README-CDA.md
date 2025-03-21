# Constrained Device Application (Connected Devices)

## Lab Module 05

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Esta implementación en la CDA añade capacidades de serialización y deserialización de datos en formato JSON para los contenedores de datos de sensores y actuadores. Además, se ha integrado una interfaz IPersistenceClient que permite la persistencia de datos en una base de datos de series temporales, como Redis o InfluxDB.

How does your implementation work?

Se ha desarrollado una clase DataUtil que maneja la conversión de objetos de datos de sensores y actuadores a formato JSON y viceversa. La interfaz IPersistenceClient se ha implementado para interactuar con una base de datos de series temporales, permitiendo almacenar y recuperar datos históricos. Esta arquitectura facilita la gestión y análisis de datos en la CDA.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/iriaagullo/python-components/tree/labmodule05

Rama: labmodule05


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest
- DataUtilTest
- SystemCpuUtilTaskTest
- SystemMemUtilTaskTest
- SensorDataTest
- ActuatorDataTest
- SystemPerformanceDataTest
- SenseHatSensorAdapterTest
- SenseHatActuatorAdapterTest
- PersistenceClientTest

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SystemPerformanceManagerTest
- SensorAdapterManagerTest
- ActuatorAdapterManagerTest
- SenseHatEmulatorIntegrationTest
- DataIntegrationTest

EOF.
