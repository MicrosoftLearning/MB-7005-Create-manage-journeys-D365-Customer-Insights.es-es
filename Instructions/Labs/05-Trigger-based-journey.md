---
lab:
  title: 'Laboratorio 4: Creación de un recorrido basado en desencadenadores'
---

## Laboratorio 4: Creación de un recorrido basado en desencadenadores 

Estos son los objetivos del laboratorio:
- Creación de un recorrido basado en desencadenadores
- Definición de los criterios de salida para el segmento 

### Tarea 1: Creación de un recorrido basado en desencadenadores 
1. Ve al área de trabajo **Recorridos en tiempo real**.

1. En **Involucración**, selecciona **Recorridos.**

1. Haz clic en **+ Nuevo recorrido** en la barra de comandos.

1. Selecciona **Omitir y crear desde cero.**

1. En **Nombre del recorrido**, escribe **Recorrido de bienvenida.**

1. En **Elegir tipo de recorrido**, selecciona **Basado en desencadenadores.**

1. En **Elegir un desencadenador**, busca y selecciona **Contacto creado.**

1. Haz clic en **Crear.**

1. En la configuración del recorrido de la derecha, en la sección Entrada, selecciona **Agregar condición.**

1. En el menú desplegable Atributo, selecciona **Contacto creado > Contacto (contacto) > Cuenta (cuenta) > Nombre de cuenta.**

1. Cambia el operador a **No es igual.**

1. Establece el valor en **Humongous Insurance**. La condición debe decir **Nombre de cuenta No es igual a Humongous Insurance.**

1. Configura el resto de los elementos de la sección Entrada de la manera siguiente:
    - En la sección **Repetir**, selecciona Inmediatamente.
    - En la sección Zona horaria, elige la zona horaria.
    - En Inicio, seleccione la fecha actual, dentro de 15 minutos.
    - En Fin, selecciona mañana.

### Tarea 2: Definición del objetivo del recorrido
A continuación, podemos identificar el objetivo específico del recorrido del cliente.  Los objetivos ayudan a identificar cuál es el punto final del recorrido.  Pueden ser cosas como impulsar una compra o interactuar con los clientes.  Proporcionar un objetivo al recorrido garantiza que este se detenga una vez que se haya cumplido el objetivo.    

En este recorrido, el objetivo es que un porcentaje específico de personas con las que interactuamos haga clic en un vínculo que se encuentra en un correo electrónico que les enviamos.  

1.  En la configuración del recorrido de la derecha, ve a la sección **Objetivo**.

1.  En **El objetivo de este recorrido es**, selecciona **Enviar una notificación general.**

1.  En el campo **El objetivo se cumple cuando,** selecciona **Una persona haga clic en al menos un vínculo.**

1.  En **La cantidad de personas necesarias,** especifica **50.** Deja seleccionada la opción **Porcentaje**. 

### Tarea 3: Definición de una frecuencia máxima para el recorrido 
Contoso quiere asegurarse de que no están agobiando a sus clientes con mensajes comerciales. Para asegurarse de que esto no sucede, quieren aplicar a este recorrido una frecuencia máxima.   

1.  En la configuración del recorrido de la derecha, ve a la sección **Otros opciones**.

1.  En Frecuencia máxima, asegúrate de que está seleccionado **Aplicar frecuencia máxima a este recorrido: omitir los mensajes comerciales si se alcanza el máximo**.  

1.  En Frecuencia máxima entre recorridos, selecciona **Ir a la configuración de la frecuencia máxima.** Se abrirá una ventana nueva.

1.  Selecciona **+ Nueva configuración** en la barra de comandos.

1.  En el campo Nombre, escribe **Contoso**.

1.  En la sección Frecuencia máxima por punto de contacto, configura en función de la imagen siguiente:

    ![Captura de pantalla de la configuración de la frecuencia máxima, correo electrónico establecido en Diario 3 y Mensual 10, mensaje de texto establecido en Diario 1, Semanal 2 y Mensual 3. No se establece nada para la notificación push.](../Labs/Media/frequency-cap.png)

1. Selecciona **Guardar y cerrar** para guardar y cerrar la nueva configuración de la frecuencia máxima.  

1.  Vuelve a la ventana que contiene el recorrido de bienvenida. **Guarda** el archivo y actualiza el explorador.

1.  En la configuración del recorrido de la derecha, vuelve a la sección **Otras opciones**.

1.  Observa que la frecuencia máxima de Contoso se aplica ahora a este recorrido.  

### Tarea 4: Creación del recorrido basado en desencadenadores 
Ahora que hemos definido los criterios necesarios del recorrido, el siguiente paso es crear los pasos concretos del recorrido. 

1. En el diseñador de recorridos, haz clic en el **icono más (+)** en el icono Contacto creado.

1. Selecciona **Rama de atributo (Rama basada en un valor específico).**

1. En Nombre para mostrar a la derecha, escribe **New Business Customer.**

1. Selecciona **Rama 1** y en **Elegir un atributo**, busca **Descripción (descripción)** en Contacto.

1. Cambia el valor de Equals a **Contains.**

1. En Valor, escribe **Business.**

1. Haz clic en el **icono más (+)** en Rama 1.

1. Selecciona **Correo electrónico: Enviar un correo electrónico.**

1. En **Seleccionar correo electrónico**, elige **Welcome Email 1.**

1. Haz clic en el **icono de más (+)** en el icono Enviar un correo electrónico.

1. Selecciona **Esperar desencadenador.**

1. Para configurar la rama If/then, en el panel de rama If/then de la derecha, en Esperar, Elegir un tipo de condición de rama selecciona El mensaje anterior obtiene una interacción.

1. En **Elegir una interacción**, selecciona **Se ha hecho clic en el vínculo del correo electrónico.**

1. En **¿Cuál es el límite de tiempo?,** escribe 10 minutos.

1. De nuevo, en el diagrama del recorrido, selecciona **crear ramas** para especificar el vínculo en el que se hace clic.

1. Selecciona el atributo **Se ha hecho clic en el vínculo del correo electrónico.**

1. En la rama 1, selecciona el botón de llamada a la acción del correo electrónico.

1. En la ruta de acceso Sí, haz clic en el **icono más (+)**.

1. Selecciona **Enviar un correo electrónico**.

1. En Seleccionar correo electrónico, elige **Welcome Email 2.**

1. En la ruta de acceso No correspondiente, haz clic en el **icono más (+).**

1. Selecciona **Enviar un correo electrónico**.

1. En Seleccionar correo electrónico, elige **Welcome Email 3.**

1. Guarda el recorrido.

1. Revisa el recorrido. Realiza los cambios finales.

1. Haz clic en **Publicar**. Espera a que se publique el recorrido.


