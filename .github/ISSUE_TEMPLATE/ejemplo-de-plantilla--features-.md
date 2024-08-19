---
name: Ejemplo de Plantilla [Features]
about: Ejemplo de una plantilla de tipo Features
title: ''
labels: ''
assignees: ''

---

<img src="https://didcom.com.mx/wp-content/uploads/2016/12/Didcom-logo.png" alt="Diagrama de flujo" width="274px" height="75px">

## **US04 [Feature] Solicitud de cambios de Firmware RPT Transportes Pitic**
---

### **Descripción:**

- **Resumen:**
    El Cliente quiere que el RPT proporcione los siguientes reportes adicionales a los ofrecidos por el RTP versión 1.02

   - Nuevos Reportes para la versión 1.04
        1. Detección del Modo de Operación
        2. Alertas por regla que avise cualquier cambio de Setpoint
        3. Alertas por regla que avise si la unidad se encuentra fuera del rango de tolerancia (5°)
        4. Alertas por regla que avise si la unidad se encuentra en defrost por más de 1 hora
 
- **Beneficio:**
  


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
 

### **Requisitos de la Nueva Característica:**
   - Nuevos Reportes para la versión 1.04
        1. Detección del Modo de Operación
        2. Alertas por regla que avise cualquier cambio de Setpoint
        3. Alertas por regla que avise si la unidad se encuentra fuera del rango de tolerancia (5°)
        4. Alertas por regla que avise si la unidad se encuentra en defrost por más de 1 hora

### **Criterios de Aceptación:**

- [ ] Detección del Modo de Operación Modo Start/Stop, Modo Continuo
- [ ] Alertas por cualquier cambio en la temperatura de consigna
- [ ] Alertas si la temperatura de retorno es mayor de 5°F a la temperatura de consigna
- [ ] Alertas si la temperatura de retorno es menor de 5°F a la temperatura de consigna.
- [ ] Alertas por regla que avise si la unidad se encuentra en deshielo por más de 1 hora

**El Desarrollador asignado deberá marcar el avance en los criterios de aceptación diariamente**

### **Comentarios Adicionales (Opcional):**

 - Considerar la lógica con la que se enviaran los datos sea igual o similar a los datos de temperatura de retorno y de consigna.
 - Considerar si para cada requerimiento se requiere de una investigación y crear los Issues suficientes para abarcar el proyecto
---

### **Etiqueta y Asignación:**

- **Etiquetas:** Feature, Solicitud del Cliente
- **Asignado a:** [Jesús Jashimoto]

---

### **Notas:**

- **Prioridad:** Media
- **Fecha límite:** [7 de Agosto del 2024]
