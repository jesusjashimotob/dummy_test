---
name: Ejemplo de Plantilla [Testing]
about: Ejemplo de una plantilla tipo [Testing]
title: ''
labels: ''
assignees: ''

---

<img src="https://didcom.com.mx/wp-content/uploads/2016/12/Didcom-logo.png" alt="Diagrama de flujo" width="274px" height="75px">

## **US04-01 [TESTING] Detección del Modo de Operación del Reefer **

---

### **Descripción:**

- **Objetivo de la Prueba:**
  Evaluar la Funcionalidad de Monitoreo de Modo de Operación

 
### **Entorno:**

- **Hardware:**
    - Tarjeta IOX-STURNUS LITE
    - GO9 conectado con cable 3 wire
    - IOX-RS232
    - MAGICAN
    - Reefer Assembly Board V1.0
    - Programador PICkit 3 o compatible

- **Versión del Firmware:**
    Versión 1..02 (se implementará en la próxima versión).

- **Software:**
  - PICC - PICWHD Compiler version 5.103
  - MPLAB IPE
  - CANCapture

- **Entorno de Pruebas:**
  - Laboratorio de pruebas internas con osciloscopio, E-COM.

### **Casos de Prueba:**

1. **Prueba de Detección de Cambios en Modo de Operación**
   - Descripción: Con un LED de pruebas detectar si el código es capaz de detectar los cambios en el modo de operación  de un recorrido, marcando con códigos de encendido el modo de operación detectado
   - Resultado Esperado: que el LED indique los pasos del proceso de detección cuando se envíen los mensajes de prueba y recorridos

2. **Prueba de Detección de Cambios en Modo de Operación criterio 2**
   - Descripción: Confirmar en GEOTABS que los datos que envió el RPT corresponda con los valores de datos enviados en la prueba 
   - Resultado Esperado: No deben producirse errores.

3. **Prueba de Detección de Cambios en Modo de Operación criterio 3:**
   - Descripción: Confirmar que si el modo de operación no cambia, se enviara cada 15 minutos a GEOTABS confirmación del estado del modo de operación.
   - Resultado Esperado: Que el modo registrado en GEOTABS  sea igual al modo de operación de la prueba.

### **Criterios de Aceptación:**

- [ ] Cada prueba debe cumplir con los resultados esperados.
- [ ] No deberán verse afectadas las funcionalidades existentes.
- [ ] Documentar los procesos y resultados de las pruebas

### **Notas Adicionales:**


---
