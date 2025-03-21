# Constrained Device Application (Connected Devices)

## Lab Module 03

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Esta implementación añade capacidades de simulación de datos y generación de datos en la CDA. Se han incorporado sensores simulados para medir la humedad, la presión y la temperatura, utilizando un generador de datos proporcionado o uno propio. Además, se ha implementado un umbral simple que, al ser superado, activa un comando de actuador simulado.

How does your implementation work?

La CDA ha sido ampliada para incluir sensores simulados que generan datos de humedad, presión y temperatura. Estos datos se empaquetan como objetos de telemetría que contienen información adicional sobre el dispositivo. Se ha implementado un disparador de umbral simple que emite un comando de actuador simulado cuando se superan ciertos límites predefinidos. Esta arquitectura modular permite una fácil extensión y mantenimiento de la aplicación.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/iriaagullo/python-components/tree/labmodule03

Rama: labmodule03

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
- SystemPerformanceDataTest

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SystemPerformanceManagerTest​
- SensorAdapterManagerTest​
- ActuatorAdapterManagerTest

EOF.
