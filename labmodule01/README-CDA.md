# Constrained Device Application (Connected Devices)

## Lab Module 01

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Nuestra implementación configura y ejecuta el entorno de desarrollo de la Constrained Device Application (CDA) utilizando el repositorio python-components. Se han seguido los pasos descritos en la documentación para garantizar una configuración adecuada, asegurando la correcta configuración del archivo ConfigConst.py y la configuración de la variable de entorno PYTHONPATH para permitir la ejecución fluida de la aplicación y sus pruebas.

How does your implementation work?

El desarrollo se centró en la verificación de la estructura del código, la correcta inicialización de la CDA y la ejecución de pruebas unitarias e integradas. Se realizó la clonación del código base, la creación de una nueva rama labmodule01 y la validación de los archivos de configuración. Posteriormente, se ejecutaron todas las pruebas para confirmar que no se introdujeron regresiones.

### Code Repository and Branch

NOTE: Be sure to include the branch 

URL: 

### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest

- DataUtilTest

- OtherTestCases...

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SensorSimAdapterManagerTest

- DeviceDataManagerTest

- ConstrainedDeviceAppTest

EOF.
