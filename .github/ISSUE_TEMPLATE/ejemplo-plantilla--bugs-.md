---
name: Ejemplo Plantilla [Bugs]
about: Ejemplo de una plantilla de tipo Bugs
title: ''
labels: ''
assignees: ''

---

<img src="https://didcom.com.mx/wp-content/uploads/2016/12/Didcom-logo.png" alt="Diagrama de flujo" width="274px" height="75px">

## **[Bug] Problema en las Temperatura de retorno y Temperatura**


---

### **Descripción:**

- **Resumen:**
   En el PRT, se ha detectado que en el módulo GEOTABS las lecturas de temperatura de retorno y temperatura de consigna están invertidas, lo que podría generar inconsistencias en la operación.


- **Impacto:**
  Genera que la información de las temperaturas no tenga una correcta correlación con la operación del reefer

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
  
### **Pasos para Reproducir (Solo para Bugs):**

1. Leer las variables en GEOTAB durante operación normal, no es necesario realizar ninguna acción adicional

### **Comportamiento Esperado:**

- El RPT debe enviar correctamente las variables a GEOTABS 

### **Comportamiento Observado:**

- El RPT en operación normal envía los valores de Temperatura de Retorno a la variable en GEOTAB temperatura de Consigna 
- El RPT en operación normal envía los valores de Temperatura de Consigna a la variable en GEOTAB Temperatura de Retorno 


### **Propuesta de Solución (Opcional):**

- En el archivo de configuración "Main.h", invertir los valores de las constantes que apuntan a las direcciones donde se envía la información de los valores de Temperatura de Consigna y Temperatura de Retorno

---

### **Criterios de Aceptación:**

- [ ] El valor de la temperatura de retorno se debe visualizar en las variables de GEOTAB en la variable temperatura de retorno.
- [ ] El valor de la temperatura de consigna se debe visualizar en las variables de GEOTAB en la variable temperatura de consigna .

### **Comentarios Adicionales (Opcional):**

- Este problema se observó en la versión 1.01.

---

### **Etiqueta y Asignación:**

- **Etiquetas:** Bug, Temperaturas Consigna y Retorno Invertidas en GEOTABS
- **Asignado a:** [Jesus Jashimoto]

---

### **Notas:**

- **Prioridad:** Alta
- **Fecha límite:** [Fecha]
