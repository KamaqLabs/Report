# **CAPÍTULO V: SOLUTION UI/UX DESIGN**

## 5.1. Style Guidelines

En esta sección se definen los estilos de diseño front-end que serán la base para dar forma a nuestro producto **IoT Hotel Management**, utilizando patrones que consideren la arquitectura de la información, la accesibilidad y la consistencia visual tanto en la **Landing Page**, la **Aplicación Web**, la **Aplicación Móvil** y las **interfaces IoT (paneles y dashboards)**.

### 5.1.1. General Style Guidelines

**Branding:**  
El branding del logo de nuestra plataforma “IoT Hotel Management” combina elementos que transmiten **innovación, seguridad y confort**, valores esenciales en la experiencia hotelera digital.  
El diseño del logotipo utiliza una tipografía moderna acompañada de un ícono alusivo a la conectividad IoT (ondas o nodos interconectados). Su forma transmite **tecnología, confiabilidad y elegancia**, reforzando la identidad de un sistema que integra gestión, automatización y hospitalidad inteligente.

<img src="/assets/Logo Dedalus.jpg">


**Typography:**  
Para la tipografía se ha seleccionado **Roboto**, por su legibilidad y adaptabilidad en diferentes dispositivos.  
Esta fuente equilibra un aspecto profesional y moderno, asegurando buena lectura en pantallas de administración (web) y en interfaces móviles para huéspedes.  
Se usa **Roboto Regular** para textos, **Roboto Medium** para subtítulos y **Roboto Bold** para títulos o botones interactivos.

<img src="/assets/Tipografia Dedalus.png">

**Colors:**  
La paleta de colores se centra en tonos **azules y grises tecnológicos**, que evocan profesionalismo, innovación y confianza, combinados con acentos cálidos en dorado o verde azulado que transmiten confort y hospitalidad.  
Los tonos claros se reservan para fondos o áreas de lectura, mientras que los tonos oscuros se aplican en paneles, encabezados y dashboards, favoreciendo el contraste visual y la legibilidad.

<img src="/assets/Colors Dedalus.png">

---

### 5.1.2 Web, Mobile and IoT Style Guidelines

Para los lineamientos visuales de **IoT Hotel Management**, se mantuvo un estilo **minimalista, funcional y moderno**, enfocado en la experiencia de uso tanto para administradores como para huéspedes.

- **Web (Administrador):** Interfaz con colores neutros, paneles laterales y componentes organizados por tarjetas. Se prioriza la lectura clara de métricas IoT y la gestión intuitiva de reservas y sensores.  
- **Mobile (Huésped):** Diseño basado en interacción táctil con íconos grandes, colores de acento cálidos y transiciones suaves para controlar iluminación, temperatura o accesos.  
- **IoT Dashboards:** Paneles visuales con indicadores en tiempo real (temperatura, ocupación, alertas), siguiendo un esquema visual claro y accesible.  

El uso de **Roboto** y la paleta azul-gris mantienen coherencia entre todas las plataformas, garantizando una identidad visual sólida y confiable.

---

## 5.2 Information Architecture

### 5.2.1 Organization Systems

- **Segmento Huésped**

    - **Registro y Acceso de Usuario:**  
      Sistema seguro que permite el ingreso mediante credenciales, NFC o Bluetooth, garantizando una experiencia fluida y personalizada.

    - **Gestión de Reservas:**  
      Permite visualizar, modificar o cancelar reservas directamente desde la aplicación móvil, con sincronización en tiempo real con el sistema web.

    - **Control de Habitación:**  
      Los huéspedes pueden controlar luces, cortinas y temperatura desde la app móvil, generando un entorno personalizado.

    - **Solicitudes de Servicio:**  
      Opción para pedir servicio a la habitación o limpieza directamente desde la aplicación, con confirmación y seguimiento.

    - **Historial de Estancia:**  
      Registro de visitas anteriores y preferencias guardadas para futuras reservas.

---

- **Segmento Hotel (Administrador)**

    - **Gestión de Habitaciones y Reservas:**  
      Permite crear, editar o eliminar habitaciones, además de manejar las reservas y disponibilidad en tiempo real.

    - **Monitoreo de Sensores:**  
      Panel de control para supervisar los sensores de humo, gas y presencia, con alertas automáticas ante incidencias.

    - **Control Energético:**  
      Módulo para visualizar el consumo energético por habitación y aplicar estrategias de ahorro automatizadas.

    - **Gestión de Ofertas y Promociones:**  
      Creación y difusión de promociones o descuentos, integradas en la app del huésped.

    - **Reportes y Analítica:**  
      Visualización de métricas operativas e IoT (energía, accesos, alertas, ocupación) mediante dashboards interactivos.

---

### 5.2.2 Labeling Systems

- **Segmento Huésped**

    - **Etiqueta de Estado de Reserva:** Indica si la reserva está confirmada, pendiente o finalizada, mostrando además las fechas de check-in/out.  
    - **Etiqueta de Dispositivos:** Muestra el estado de conexión de luces, cortinas o termostatos (encendido, apagado, automático).  
    - **Etiqueta de Solicitudes:** Refleja el estado de pedidos de servicio (pendiente, en proceso, completado).  
    - **Etiqueta de Alertas:** Notifica si existen incidencias de humo, gas o mantenimiento en curso.  

- **Segmento Hotel**

    - **Etiqueta de Habitación:** Muestra disponibilidad, ocupación y estado de sensores.  
    - **Etiqueta de Energía:** Visualiza consumo por habitación o piso.  
    - **Etiqueta de Alertas IoT:** Informa en tiempo real sobre incidentes detectados.  
    - **Etiqueta de Tareas:** Lista las actividades asignadas al personal en respuesta a alertas o pedidos de huéspedes.

---

### 5.2.3 SEO Tags and Meta Tags

Para la optimización de búsqueda en motores web, se definen las siguientes etiquetas:

- **Title:** IoT Hotel Management  
- **Meta Tags:**  
    - **Description:** Plataforma integral de gestión hotelera con automatización IoT, sensores inteligentes y control de habitaciones desde app y web.  
    - **Keywords:** hoteles inteligentes, IoT, reservas, automatización, sensores, control de energía, hotel management.  
    - **Author:** IoT Hotel Management Team  

---

### 5.2.4 Searching Systems

- **Segmento Huésped**

    - **Búsqueda por Palabras Clave:** Permite buscar hoteles, habitaciones o servicios disponibles.  
    - **Búsqueda por Filtros:** Incluye filtros por ubicación, precio, tipo de habitación, servicios IoT disponibles (luces, climatización).  

- **Segmento Hotel**

    - **Búsqueda por Palabras Clave:** Permite al personal ubicar rápidamente huéspedes, reservas o habitaciones específicas.  
    - **Búsqueda por Filtros:** Permite refinar resultados según estado de ocupación, tipo de sensor o rango de consumo energético.

---

### 5.2.5 Navigation Systems

- **Segmento Huésped**

    - **Menú de Navegación:** Barra inferior con accesos rápidos a control de habitación, reservas, pedidos y perfil.  
    - **Enlaces Rápidos:** Accesos directos a funciones críticas como check-in/out, soporte y promociones activas.  

- **Segmento Hotel**

    - **Panel de Navegación:** Barra lateral izquierda con secciones para gestión de reservas, monitoreo IoT, energía y reportes.  
    - **Atajos Operativos:** Botones rápidos para responder alertas, asignar tareas o revisar el estado de habitaciones.  


## 5.3 Landing Page UI Design 
### 5.3.1 Landing Page Wireframe

<img src="../assets/Wireframe Landing 1.png">
<img src="../assets/Wireframe Landing 2.png">
<img src="../assets/Wireframe Landing 3.png">

### 5.3.2 Landing Page Mock-up

<img src="../assets/Wireframe Landing 1.png">
<img src="../assets/Wireframe Landing 2.png">
<img src="../assets/Wireframe Landing 3.png">

## 5.4 Applications UX/UI Design

### 5.4.1 Applications Wireframes

<img src="/assets/Wireframe1.png">


### 5.4.2 Applications Wireflow Diagrams

- **User Goal 1: Iniciar sesión**
<br>
<img src="../assets/UserGoal1.png">

- **User Goal 2: Asignar una tarea a un empleado**
<br>
<img src="../assets/UserGoal2.png">

- **User Goal 3: Añadir una reserva**
<br>
<img src="../assets/UserGoal4.png">

- **User Goal 4: Modificar una reserva existente**
<br>
<img src="../assets/UserGoal5.png">

- **User Goal 5: Cancelar una reserva**
<br>
<img src="../assets/UserGoal6.png">

- **User Goal 6: Generar reportes de estadísticas personalizadas**
<br>
<img src="../assets/UserGoal7.png">

#### 5.4.2.1 Applications Mock-ups

<img src="/assets/Mockup1.png">
<img src="/assets/Mockup2.png">
<img src="/assets/Mockup3.png">
<img src="/assets/Mockup4.png">
<img src="/assets/Mockup5.png">


### 5.4.3 Applications User Flow Diagrams

<img src="../assets/UserFlow1-Dedalus.png">
<img src="../assets/UserFlow2-Dedalus.png">
<img src="../assets/UserFlow3-Dedalus.png">
<img src="../assets/UserFlow4-Dedalus.png">
<img src="../assets/UserFlow5-Dedalus.png">
<img src="../assets/UserFlow6-Dedalus.png">


## 5.5 Applications Prototyping

<a href="https://youtu.be/DpDvyiFZYfk" target="_blank">
  <img src="../assets/Prototyping-Dedalus.png" alt="Haz clic para ver el video en YouTube">
</a>

Link de figma: https://www.figma.com/design/bbKcl86Op3sFtBF6jHzzG0/Dedalus-MuckUps?node-id=2001-1221&t=LA4A0IOFnLQJ93jI-1