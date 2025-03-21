# Constrained Device Application (Connected Devices)

## Lab Module 04

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Esta implementación integra la funcionalidad de sensores y actuadores utilizando el emulador Sense HAT en la CDA. Se han incorporado sensores para medir la humedad, la presión y la temperatura, y se ha implementado un actuador que interactúa con la pantalla LED del emulador para mostrar mensajes o estados específicos.

How does your implementation work?

La CDA ha sido ampliada para interactuar con el emulador Sense HAT, permitiendo la lectura de datos de sensores y el control de actuadores. Los datos de los sensores se recopilan y procesan en tiempo real, y el actuador controla la pantalla LED del emulador para mostrar información relevante o alertas basadas en los datos recopilados. Esta integración permite una simulación realista de un entorno IoT, facilitando el desarrollo y prueba de funcionalidades sin necesidad de hardware físico.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/iriaagullo/python-components/tree/labmodule04

Rama: labmodule04


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest​
- DataUtilTest​
- SystemCpuUtilTaskTest​
- SystemMemUtilTaskTest​
- SensorDataTest​
- ActuatorDataTest​
- SystemPerformanceDataTest​
- SenseHatSensorAdapterTest​
- SenseHatActuatorAdapterTest

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SystemPerformanceManagerTest​
- SensorAdapterManagerTest​
- ActuatorAdapterManagerTest​
- SenseHatEmulatorIntegrationTest

EOF.
