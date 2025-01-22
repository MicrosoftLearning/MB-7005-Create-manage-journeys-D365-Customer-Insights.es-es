---
lab:
  title: 'Laboratorio 2: Creación de segmentos'
---

## Laboratorio 2: Creación de segmentos 

Estos son los objetivos del laboratorio:
- Actualización de la información sobre los registros de clientes
- Creación de un segmento 

### Tarea 1: Actualización de la ciudad de diferentes clientes

Uno de los recorridos está dirigido a los clientes que viven en una ciudad específica. Para asegurarte de que tendrás miembros en este segmento, necesitarás agregar una ciudad a cada uno de los contactos que existen actualmente.

1. Inicia sesión en **Dynamics 365 Customer Insights - Journeys**. Asegúrate de que te encuentras en el área **Recorridos en tiempo real**.

1. En Audiencia, selecciona **Contactos.**

1. Selecciona los primeros 10 contactos de la lista. 

1. En la barra de comandos, selecciona **Editar**.

1. En el campo Dirección 1: Ciudad, escribe **Seattle.**

1. Selecciona el botón **Guardar**.

1. Selecciona los 50 contactos siguientes de la lista.

1. En la barra de comandos, selecciona **Editar**.

1. En el campo Dirección 1: Ciudad, escribe **Portland.**

1. Selecciona el botón **Guardar**.

1. Selecciona los 10 contactos siguientes de la lista.

1. En la barra de comandos, selecciona **Editar**.

1. En el campo Dirección 1: Ciudad, escribe **Boise.**

1. Selecciona el botón **Guardar**.

1. Selecciona los 10 contactos siguientes de la lista.

1. En la barra de comandos, selecciona **Editar**.

1. En el campo Dirección 1: Ciudad, escribe **Seattle.**

1. Cambia a la pestaña **Detalles**. En el cuadro de texto de **Notas personales**, escribe **Business.**

1. Selecciona el botón **Guardar**.

### Tarea 2: Creación de un segmento para los clientes de Humongous Insurance

1. Ve a **Segmentos**, en el grupo Audiencia.

1. Selecciona **+ Nuevo segmento**.

1. En el cuadro **Nombre del segmento**, escribe **Humongous Insurance**. Selecciona **Contacto** como audiencia objetivo. Selecciona **Crear**.

1. Selecciona **Agregar un nuevo grupo** en el diseñador de segmentos. Primero, elegiremos un **Grupo de atributos.**

1. En el panel Atributos, expande **Contacto** y selecciona **Cuenta**. Agrega el elemento al grupo existente.

1. En la búsqueda del Grupo 1, selecciona **Humongous Insurance.** La condición del Grupo 1 dirá "La cuenta es Humongous Insurance".

1. Queremos agregar otra condición al segmento. Selecciona **+Agregar nuevo** para agregar un nuevo grupo y selecciona **Grupo de atributos.**

1. Cambia el operador a **or.**
    - En el panel Atributos, empieza a escribir **Correo electrónico.** Expande **Contacto.** Selecciona el botón **más** situado junto al campo correo electrónico y agrégalo al Grupo 2.
    - Crea la siguiente condición: **El correo electrónico contiene humongousinsurance**

1. Selecciona **Guardar.**

1. Selecciona **Listo para usar** en la barra de herramientas.

1. Selecciona la pestaña **Miembros e información**. Comprueba que ves los contactos con un correo electrónico de Humongous Insurance o con el nombre de empresa de Humongous. Es posible que tengas que actualizar o esperar unos minutos antes de que aparezcan los contactos.

### Tarea 3: Creación de un segmento de usuario profesional

1. Ve a **Segmentos** en el grupo Audiencia.

1. Selecciona **+ Nuevo segmento**.

1. Denomina el segmento **Business Customers**. Mantén **Contacto** seleccionado como Audiencia objetivo. Selecciona **Crear**.

1. En el panel **Atributos**, expande **Contacto** y selecciona **Cuenta**. Agrega el elemento al grupo existente.

1. En la búsqueda del Grupo 1, selecciona **Contoso, Ltd.**

1. Selecciona **Guardar** y luego elige **Listo para usar.**

1. Espera a que el segmento se cree.

1. Selecciona la pestaña **Miembros e información** para ver los miembros del segmento.

### Tarea 4: Creación de un segmento de Contoso  
2.  Ve a **Segmentos** en el grupo Audiencia. 

3.  Selecciona **+ Nuevo segmento. **

4.  Denomina el segmento **Clientes de Contoso**. Mantén **Contacto** seleccionado como Audiencia objetivo. Selecciona **Crear**.

5.  Agrega un nuevo grupo y selecciona **Crear grupo de atributos**. En el panel **Atributos**, expande **Contacto** y agrega **Descripción** al Grupo 1. 

6.  En el diseñador de segmentos, cambia el calificador a **Contains**. Para el valor, escribe **Business.**

7.  Selecciona **Guardar** y luego elige **Listo para usar.** 

8.  Espera a que el segmento se cree. 

9.  Selecciona la pestaña **Miembros e información** para ver los miembros del segmento. 


### Tarea 5: Creación de un segmento de clientes de Seattle
1. Ve a Segmentos en el grupo Audiencia.

1. Selecciona **+ Nuevo segmento**.

1. Denomina el segmento **Seattle Customers**. Mantén **Contacto** seleccionado como Audiencia objetivo.

1. Selecciona el botón **Crear**.

1. Agrega un nuevo grupo y selecciona **Crear grupo de atributos**. En el panel Atributos, expande **Contacto > Dirección 1** y agrega **Dirección 1: Ciudad** al Grupo 1.

1. En el diseñador de segmentos, deja el calificador tal cual. Para el valor, escribe **Seattle.**

1. Selecciona **Guardar** y luego elige **Listo para usar.**

1. Espera a que el segmento se cree.

1. Selecciona la pestaña **Miembros e información** para ver los miembros del segmento.
