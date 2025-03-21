# Gateway Device Application (Connected Devices)

## Lab Module 02

Be sure to implement all the PIOT-GDA-* issues.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

La implementación de la GDA se encarga de recopilar y gestionar datos de rendimiento del sistema en un dispositivo gateway. La aplicación monitorea métricas esenciales como la utilización de la CPU y la memoria, registrando estos datos a intervalos regulares para garantizar un funcionamiento eficiente y la detección temprana de posibles problemas de rendimiento.

How does your implementation work?

La GDA está desarrollada en Java y emplea clases dedicadas para la recopilación de datos del sistema. Se implementa un gestor de rendimiento del sistema que programa tareas de monitoreo en intervalos específicos. Estas tareas recopilan datos de utilización de la CPU y la memoria, los cuales se registran utilizando el sistema de logging de Java. La estructura modular de la aplicación facilita su escalabilidad y mantenimiento.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/iriaagullo/java-components/tree/labmodule02

Rama: labmodule02

### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest​
- DataUtilTest​
- SystemCpuUtilTaskTest​
- SystemMemUtilTaskTest

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SystemPerformanceManagerTest

EOF.
