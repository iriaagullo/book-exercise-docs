# Constrained Device Application (Connected Devices)

## Lab Module 02

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

La implementación de la CDA se centra en la recopilación y gestión de datos de rendimiento del sistema en un dispositivo con recursos limitados. La aplicación monitorea métricas clave como la utilización de la CPU y la memoria, registrando estos datos a intervalos regulares para su posterior análisis y optimización del rendimiento.

How does your implementation work?

La CDA está desarrollada en Python y utiliza módulos especializados para la recopilación de datos del sistema. Se implementa un gestor de rendimiento del sistema que programa tareas de monitoreo en intervalos definidos. Estas tareas recopilan datos de utilización de la CPU y la memoria, los cuales se almacenan y registran utilizando el sistema de logging integrado. Esta arquitectura modular permite una fácil extensión y mantenimiento de la aplicación.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/iriaagullo/python-components/tree/labmodule02

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
