# **RELACIÓN FINAL DE EJERCICIOS DOM**

<center>
  <img src="dom2.webp" alt="Representación del DOM y creación dinámica" width="300">
</center>

#### **1. Validación en Tiempo Real de Formularios con Mensajes de Error**

- **Enunciado**: Crea un formulario con un campo de email. Valida en tiempo real si el usuario ha introducido un correo válido (con formato correcto de email). Si el email no es válido, muestra un mensaje de error dinámico bajo el campo de texto.
- **Conceptos clave**: `input`, `addEventListener`, `regex`, `createElement`, `appendChild`, `remove`.
- **Ejemplo**: Detectar la validez del correo electrónico mientras el usuario escribe y mostrar/ocultar un mensaje de error.

#### **2. Crear un Sistema de Pestañas (Tabs) Dinámico**

- **Enunciado**: Crea una interfaz de pestañas (tabs) en la que al hacer clic en cada pestaña se muestre el contenido correspondiente, ocultando el de las otras pestañas. Todo el contenido debe generarse dinámicamente, incluyendo las pestañas y las secciones.
- **Conceptos clave**: `querySelectorAll`, `addEventListener`, `classList.add`, `classList.remove`, `createElement`.
- **Ejemplo**: Una interfaz con categorías ("Deportes", "Noticias", "Cultura") que al hacer clic en cada pestaña muestre el contenido respectivo.

#### **3. Drag and Drop para una Lista Ordenable**

- **Enunciado**: Implementa una lista de elementos que el usuario pueda reordenar arrastrando y soltando (drag and drop). Asegúrate de que el nuevo orden se refleje en un array subyacente.
- **Conceptos clave**: `dragstart`, `dragover`, `drop`, `insertBefore`, sincronización con estructuras de datos.
- **Ejemplo**: Una lista de tareas ("Estudiar", "Hacer ejercicio", "Comprar comida") puede reordenarse manualmente mediante drag and drop, y el nuevo orden se guarda en un array.

#### **4. Generar una Tabla Dinámica con Contenido de un Array**

- **Enunciado**: Dado un array de objetos con datos de usuarios (nombre, edad, email), genera una tabla dinámica en la que cada fila corresponda a un usuario. Añade funcionalidad para ordenar las filas por nombre o edad cuando el usuario haga clic en los encabezados de columna.
- **Conceptos clave**: `createElement`, `appendChild`, `innerHTML`, `sort`, `addEventListener`.
- **Ejemplo**: Mostrar datos tabulados de usuarios y permitir ordenarlos dinámicamente al hacer clic en el encabezado de la tabla.

#### **5. Filtro Dinámico de Productos**

- **Enunciado**: Crea una lista de productos que se filtre dinámicamente a medida que el usuario escribe en un campo de búsqueda. Cada producto debe ser un componente generado dinámicamente a partir de un array inicial.
- **Conceptos clave**: `input`, `filter`, `querySelectorAll`, `forEach`, creación de componentes.
- **Ejemplo**: Una lista de productos como "Laptop", "Smartphone" y "Tablet" se actualiza en tiempo real a medida que el usuario escribe en la barra de búsqueda.

#### **6. Creación de un Carrito de Compras Dinámico**

- **Enunciado**: Implementa una lista de productos con un botón de "Agregar al carrito" en cada producto. Muestra un carrito que se actualiza en tiempo real con los productos seleccionados y el precio total. Permite eliminar productos del carrito.
- **Conceptos clave**: `createElement`, `appendChild`, `querySelector`, `addEventListener`, sincronización del DOM.
- **Ejemplo**: Un carrito de compras que muestra "Laptop - $1000" y "Teléfono - $500", con un total de "$1500". Los productos pueden agregarse o eliminarse dinámicamente.

#### **7. Creación de un Modal de Confirmación antes de Eliminar un Elemento**

- **Enunciado**: Crea una lista de elementos con un botón de "Eliminar" al lado de cada uno. Al hacer clic en el botón, debe aparecer un modal de confirmación que pregunte si el usuario realmente quiere eliminar el elemento.
- **Conceptos clave**: `createElement`, `appendChild`, `addEventListener`, `remove`, `preventDefault`.
- **Ejemplo**: Una lista con elementos como "Tarea 1", "Tarea 2", y "Tarea 3". Al hacer clic en "Eliminar", aparece un modal que permite confirmar o cancelar la acción.

#### **8. Creación de un Cronómetro con Funciones de Iniciar, Pausar y Reiniciar**

- **Enunciado**: Implementa un cronómetro funcional que el usuario pueda iniciar, pausar y reiniciar. El tiempo debe mostrarse en pantalla en tiempo real, actualizado cada segundo.
- **Conceptos clave**: `setInterval`, `clearInterval`, `addEventListener`, manipulación del DOM.
- **Ejemplo**: Un cronómetro que comienza en "00:00", puede pausarse en "00:45", y reiniciarse a "00:00".

#### **9. Barra de Progreso Dinámica Basada en la Entrada del Usuario**

- **Enunciado**: Crea un componente de barra de progreso que refleje visualmente el porcentaje de caracteres introducidos en un campo de texto con respecto a un límite máximo. Incluye un contador numérico junto a la barra.
- **Conceptos clave**: `input`, `setAttribute`, manipulación de atributos y DOM, creación de componentes.
- **Ejemplo**: Un campo de texto con un límite de 200 caracteres muestra una barra de progreso al 50% y un contador que dice "Caracteres restantes: 100" tras escribir 100 caracteres.

#### **10. Integración de la API de Geolocalización del Navegador**

- **Enunciado**: Utiliza la API de Geolocalización para obtener la ubicación actual del usuario y mostrarla en pantalla. Implementa un botón para actualizar la ubicación cuando el usuario lo desee.
- **Conceptos clave**: `navigator.geolocation`, `getCurrentPosition`, `innerText`, creación dinámica de elementos.
- **Ejemplo**: Al hacer clic en un botón, el navegador obtiene la ubicación del usuario ("Latitud: 40.4168, Longitud: -3.7038") y la muestra en la página.

#### **11. Generar y Descargar un Archivo de Texto con Contenido Dinámico**

- **Enunciado**: Implementa un botón que, al hacer clic, genere y descargue un archivo `.txt` con contenido dinámico, como los datos ingresados por el usuario en un formulario.
- **Conceptos clave**: `createElement`, `Blob`, `URL.createObjectURL`, interacción con el DOM.
- **Ejemplo**: Un formulario donde el usuario escribe su nombre y dirección genera un archivo "datos.txt" con esa información al hacer clic en el botón.

### **12. Creación de una Galería de Imágenes Dinámica con Lightbox**

- **Enunciado**: Crea un componente de galería de imágenes que se genere dinámicamente a partir de un array de URLs. Al hacer clic en una imagen, debe abrirse un modal (lightbox) mostrando la imagen en tamaño completo, con botones para navegar a la imagen anterior o siguiente en la galería.
- **Conceptos clave**: `createElement`, `appendChild`, manejo de eventos `click`, manipulación de clases, navegación entre imágenes.
- **Ejemplo**: Una galería de miniaturas que muestra imágenes como "imagen1.jpg", "imagen2.jpg", etc. Al hacer clic en una miniatura, se abre un lightbox mostrando la imagen ampliada, con opciones para pasar a la siguiente o anterior.

### **13. Formulario Dinámico con Campos Personalizables**

- **Enunciado**: Crea un componente de formulario que se genere dinámicamente a partir de un array de configuraciones de campos. Cada configuración debe especificar el tipo de campo (texto, número, email, etc.), el texto del `placeholder`, y si es obligatorio. El formulario debe validar los campos al enviarse y mostrar mensajes de error específicos para cada uno.
- **Conceptos clave**: `createElement`, `appendChild`, validación de formularios con `input` y `submit`, configuración dinámica de atributos.
- **Ejemplo**: Un formulario generado a partir de un array con configuraciones como `{ tipo: 'texto', placeholder: 'Nombre', requerido: true }`. Al enviarlo, valida cada campo y muestra errores si no se cumple alguna regla.

### **14. Lista de Comentarios con Función de Respuesta y Eliminación**

- **Enunciado**: Crea un componente que permita gestionar una lista de comentarios. Cada comentario debe tener un botón de "Responder" que abra un campo de texto debajo del comentario para escribir una respuesta. También debe incluir un botón de "Eliminar" para borrar el comentario o la respuesta.
- **Conceptos clave**: `createElement`, `appendChild`, manejo de eventos `click`, estructura jerárquica de elementos.
- **Ejemplo**: Una lista que muestra comentarios como "Comentario 1". Al hacer clic en "Responder", aparece un campo de texto para escribir una respuesta como "Respuesta al comentario 1". Ambos elementos pueden eliminarse independientemente.

---

### **15. Creación de una Encuesta Dinámica con Resultados en Tiempo Real**

- **Enunciado**: Crea un componente de encuesta con opciones generadas dinámicamente a partir de un array de preguntas y respuestas posibles. Cada vez que el usuario selecciona una respuesta, muestra los resultados acumulados en tiempo real en un gráfico de barras simple.
- **Conceptos clave**: `createElement`, manipulación del DOM en tiempo real, cálculo de porcentajes, representación gráfica sencilla.
- **Ejemplo**: Una encuesta con la pregunta "¿Cuál es tu lenguaje favorito?" y opciones como "JavaScript", "Python", y "Java". Al seleccionar "JavaScript", el gráfico de barras muestra los votos acumulados para cada opción.
