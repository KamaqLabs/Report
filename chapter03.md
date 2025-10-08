# Capítulo III: Requirements Specification

## 3.1. User Stories.

Las User Stories son una herramienta fundamental para definir los requisitos del proyecto. Cada User Story incluye criterios de aceptación que deben ser comprobables y redactados en tiempo presente, tercera persona, siguiendo la estructura de Gherkin (Given-When-Then). Además, se consideran User Stories para el sitio web estático (Landing Page) y Technical Stories para los features del RESTful API.

### Épicas del Proyecto
- **EPIC001 – Gestión de Habitaciones y Reservas**  
- **EPIC002 – Accesos Seguros e IoT (cerraduras, credenciales NFC/Bluetooth)**  
- **EPIC003 – Automatización de Ambiente (luces, cortinas, termostato)**  
- **EPIC004 – Seguridad y Sensores Inteligentes (humo, gas, notificaciones)**  
- **EPIC005 – Creación de la Landing Page**  

---

### EPIC001 – Gestión de Habitaciones y Reservas
| **Story ID** | **Título**               | **Descripción**                                                                                      | **Criterios de Aceptación**                                                                                                                                           | **Relacionado con (Epic ID)** |
|--------------|--------------------------|------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------|
| US001        | Crear habitación         | Como *administrador*, quiero crear habitaciones en el sistema, para gestionar disponibilidad.        | Dado que el administrador accede al panel web, cuando selecciona "Crear Habitación", entonces el sistema debe registrar la nueva habitación con los datos ingresados. | EPIC001                       |
| US002        | Editar habitación        | Como *administrador*, quiero editar habitaciones, para actualizar datos como tipo o estado.          | Dado que el administrador selecciona una habitación existente, cuando actualiza los campos, entonces el sistema debe guardar los cambios correctamente.               | EPIC001                       |
| US003        | Eliminar habitación      | Como *administrador*, quiero eliminar habitaciones, para mantener actualizado el inventario.         | Dado que el administrador selecciona una habitación, cuando confirma la eliminación, entonces esta debe desaparecer de la lista.                                      | EPIC001                       |
| US004        | Crear/gestionar reservas | Como *administrador*, quiero crear, modificar y cancelar reservas, para evitar sobreasignaciones.    | Dado que el administrador accede al módulo de reservas, cuando gestiona una reserva, entonces el sistema debe reflejar el cambio en la disponibilidad.                | EPIC001                       |
| US005        | Reporte de ocupación     | Como *administrador*, quiero ver un reporte de ocupación de habitaciones, para optimizar la gestión. | Dado que el administrador solicita el reporte, cuando se genera, entonces debe mostrar porcentaje de ocupación y reservas activas.                                    | EPIC001                       |

---

### EPIC002 – Accesos Seguros e IoT
| **Story ID** | **Título**                       | **Descripción**                                                                                           | **Criterios de Aceptación**                                                                                                           | **Relacionado con (Epic ID)** |
|--------------|----------------------------------|-----------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|-------------------------------|
| US006        | Acceso con NFC                   | Como *huésped*, quiero abrir mi habitación con NFC, para ingresar sin usar llave física.                  | Dado que el huésped tiene credenciales válidas, cuando acerca el móvil al lector, entonces la cerradura debe abrirse.                 | EPIC002                       |
| US007        | Acceso con Bluetooth             | Como *huésped*, quiero abrir mi habitación con Bluetooth, para acceder sin tarjeta.                       | Dado que el huésped tiene acceso activo, cuando se conecta vía Bluetooth, entonces el sistema debe desbloquear la cerradura.          | EPIC002                       |
| US008        | Uso de tarjeta física            | Como *huésped*, quiero usar tarjeta física, para entrar en caso de no tener NFC/Bluetooth.                | Dado que el huésped recibe tarjeta física, cuando la desliza en la cerradura, entonces debe abrirse la puerta.                        | EPIC002                       |
| US009        | Revocación de acceso en checkout | Como *administrador*, quiero que los accesos digitales se revocan en checkout, para garantizar seguridad. | Dado que el huésped hace checkout, cuando finaliza su estancia, entonces el sistema debe desactivar sus credenciales.                 | EPIC002                       |
| US010        | Registro de accesos              | Como *administrador*, quiero ver un historial de accesos, para auditar la seguridad.                      | Dado que el administrador accede al panel, cuando consulta accesos, entonces el sistema debe mostrar fecha, hora y método de entrada. | EPIC002                       |

---

### EPIC003 – Automatización de Ambiente
| **Story ID** | **Título**                  | **Descripción**                                                                                          | **Criterios de Aceptación**                                                                                                    | **Relacionado con (Epic ID)** |
|--------------|-----------------------------|----------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|-------------------------------|
| US011        | Control de luces            | Como *huésped*, quiero encender y apagar las luces desde la app, para ajustar el ambiente.               | Dado que el huésped accede a la app, cuando activa o desactiva las luces, entonces el cambio debe reflejarse en la habitación. | EPIC003                       |
| US012        | Control de cortinas         | Como *huésped*, quiero abrir o cerrar cortinas desde la app, para personalizar la iluminación.           | Dado que el huésped está en la app, cuando selecciona "Abrir/Cerrar Cortinas", entonces estas deben responder en tiempo real.  | EPIC003                       |
| US013        | Control de temperatura      | Como *huésped*, quiero regular el termostato desde la app, para tener confort climático.                 | Dado que el huésped accede al control, cuando ajusta la temperatura, entonces el termostato debe actualizarse.                 | EPIC003                       |
| US014        | Escena de bienvenida        | Como *administrador*, quiero que al check-in se activen luces y clima, para recibir al huésped.          | Dado que se activa un check-in, cuando el huésped ingresa, entonces el sistema debe aplicar la escena configurada.             | EPIC003                       |
| US015        | Escena de ahorro energético | Como *administrador*, quiero que luces y clima se apaguen al detectar desocupación, para reducir costos. | Dado que no se detecta ocupación, cuando la habitación queda vacía, entonces el sistema debe apagar luces y climatización.     | EPIC003                       |

---

### EPIC004 – Seguridad y Sensores Inteligentes
| **Story ID** | **Título**                      | **Descripción**                                                                                      | **Criterios de Aceptación**                                                                                              | **Relacionado con (Epic ID)** |
|--------------|---------------------------------|------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------|-------------------------------|
| US016        | Detección de humo               | Como *administrador*, quiero recibir alertas de humo, para actuar rápidamente.                       | Dado que un sensor detecta humo, cuando se activa, entonces el sistema debe enviar alerta inmediata al panel y app.      | EPIC004                       |
| US017        | Detección de gas                | Como *administrador*, quiero recibir alertas de gas, para evitar emergencias.                        | Dado que un sensor detecta gas, cuando el nivel es alto, entonces debe generar alerta inmediata.                         | EPIC004                       |
| US018        | Notificación en tiempo real     | Como *huésped*, quiero recibir notificaciones de seguridad, para sentirme protegido.                 | Dado que ocurre un incidente, cuando se emite una alerta, entonces el huésped debe recibir notificación push en su app.  | EPIC004                       |
| US019        | Registro histórico de alertas   | Como *administrador*, quiero consultar historial de alertas, para tener trazabilidad.                | Dado que accedo al módulo de seguridad, cuando pido historial, entonces el sistema debe mostrar fecha, tipo y respuesta. | EPIC004                       |
| US020        | Integración con tareas de staff | Como *administrador*, quiero que alertas IoT generen tareas automáticas, para acelerar la respuesta. | Dado que se activa una alerta, cuando esta se recibe, entonces debe asignarse una tarea al personal correspondiente.     | EPIC004                       |

---

### EPIC005 – Creación de la Landing Page
| **Story ID** | **Título**                 | **Descripción**                                                                                                 | **Criterios de Aceptación**                                                                                                                                                                                                                                                                                                                                   | **Relacionado con (Epic ID)** |
|--------------|----------------------------|-----------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------|
| US021        | Página inicial             | Como *visitante*, quiero ver la página inicial, para obtener una visión general del sistema.                    | Dado que accedo al sitio, cuando cargo la landing, entonces debe mostrar una introducción clara al producto. <br><br> Dado que accede al sitio, cuando visualiza el encabezado, entonces debe poder navegar hacia las secciones principales del sitio.                                                                                                        | EPIC005                       |
| US022        | Sección Proyecto	          | Como *visitante*, quiero ver las características del sistema, para entender sus beneficios.                     | Dado que accede a la sección de características, cuando navega por la landing, entonces debe visualizar una lista de funcionalidades clave del sistema.<br><br> Dado que accede a la sección de características, cuando se muestra el contenido, entonces debe incluir información sobre automatización, dashboard en tiempo real, automatización y sensores. | EPIC005                       |
| US023        | Sección de contacto        | Como *visitante*, quiero enviar un mensaje desde la landing, para solicitar más información.                    | Dado que completo el formulario, cuando lo envío, entonces el sistema debe registrar el mensaje y confirmarlo.<br><br> Dado que accede a la sección de contacto, cuando visualiza la información, entonces debe poder ver datos de contacto como dirección, teléfono y redes sociales.                                                                        | EPIC005                       |
| US024        | Sección de planes          | Como *visitante*, quiero ver los planes de suscripción, para conocer opciones de precios.                       | Dado que accedo a "Planes de Pago", cuando se muestra  el contenido, entonces debe listar los precios y modalidades disponibles.<br><br>  Dado que accede a los planes, cuando compara las opciones, entonces debe poder identificar diferencias entre los planes Básico, Pro y Empresarial.                                                                  | EPIC005                       |
| US025        | Llamada a la acción (CTA)  | Como *visitante*, quiero tener un botón de "Probar ahora", para dirigirse a la plataforma.                      | Dado que accedo a la landing, cuando hago clic en CTA, entonces debe redirigirme al Web Application.                                                                                                                                                                                                                                                          | EPIC005                       |
| US026        | Seccion About the Product  | Como *visitante*, quiero conocer detalles técnicos del producto, para evaluar su utilidad.                      | Dado que accede a la sección del producto, cuando se muestra la información, entonces debe incluir una descripción sobre cómo mejora la gestión hotelera.                                                                                                                                                                                                     | EPIC005                       |
| US027        | Seccion About The Team     | Como *visitante*, quiero conocer al equipo detrás del sistema, para confiar en el producto.                     | Dado que accede a la sección del equipo, cuando se muestra el contenido, entonces debe incluir nombres y roles de los miembros del equipo.                                                                                                                                                                                                                    | EPIC005                       |
| US028        | Seccion Miembros del grupo | Como *visitante*, quiero ver los perfiles de los desarrolladores, para saber quiénes están detrás del proyecto. | Dado que accede a la sección de miembros, cuando se muestra la información, entonces debe incluir nombres, fotografías y enlaces a redes sociales.                                                                                                                                                                                                            | EPIC005                       |
| US029        | Seccio Footer              | Como *visitante*, quiero ver el footer en la página para ver los derechos de autor.                             | Dado que navega por la landing, cuando llega al final de la página, entonces debe ver el footer con enlaces a políticas de privacidad, términos de uso y derechos de autor                                                                                                                                                                                    | EPIC005                       |


## 3.2. Impact Mapping.

##### Segmento 1: Empresas Hoteleras
![Impact Map Empresas Hoteleras](/assets/Impact%20map%20Admin.png)

##### Segmento 2: Huespedes
![Impact Map Huespedes](/assets/Impact%20map%20huesped.png)

## 3.3 Product Backlog

| **Orden** | **User Story** | **Título**                                | **Descripción** | **Story Points** |
|-----------|----------------|-------------------------------------------|-----------------|------------------|
| 1         | US001          | Crear habitación                          | Como administrador, quiero crear habitaciones en el sistema, para gestionar disponibilidad. | 3 |
| 2         | US002          | Editar habitación                         | Como administrador, quiero editar habitaciones, para actualizar datos como tipo o estado. | 2 |
| 3         | US003          | Eliminar habitación                       | Como administrador, quiero eliminar habitaciones, para mantener actualizado el inventario. | 2 |
| 4         | US004          | Gestionar reservas                        | Como administrador, quiero crear, modificar y cancelar reservas, para evitar sobreasignaciones. | 5 |
| 5         | US005          | Reporte de ocupación                      | Como administrador, quiero ver un reporte de ocupación de habitaciones, para optimizar la gestión. | 3 |
| 6         | US006          | Acceso con NFC                            | Como huésped, quiero abrir mi habitación con NFC, para ingresar sin usar llave física. | 5 |
| 7         | US007          | Acceso con Bluetooth                      | Como huésped, quiero abrir mi habitación con Bluetooth, para acceder sin tarjeta. | 5 |
| 8         | US008          | Uso de tarjeta física                     | Como huésped, quiero usar tarjeta física, para entrar en caso de no tener NFC/Bluetooth. | 2 |
| 9         | US009          | Revocación de acceso en checkout          | Como administrador, quiero que los accesos digitales se revocan en checkout, para garantizar seguridad. | 3 |
| 10        | US010          | Registro de accesos                       | Como administrador, quiero ver un historial de accesos, para auditar la seguridad. | 3 |
| 11        | US011          | Control de luces                          | Como huésped, quiero encender y apagar las luces desde la app, para ajustar el ambiente. | 3 |
| 12        | US012          | Control de cortinas                       | Como huésped, quiero abrir o cerrar cortinas desde la app, para personalizar la iluminación. | 3 |
| 13        | US013          | Control de temperatura                    | Como huésped, quiero regular el termostato desde la app, para tener confort climático. | 5 |
| 14        | US014          | Escena de bienvenida                      | Como administrador, quiero que al check-in se activen luces y clima, para recibir al huésped. | 3 |
| 15        | US015          | Escena de ahorro energético               | Como administrador, quiero que luces y clima se apaguen al detectar desocupación, para reducir costos. | 5 |
| 16        | US016          | Detección de humo                         | Como administrador, quiero recibir alertas de humo, para actuar rápidamente. | 5 |
| 17        | US017          | Detección de gas                          | Como administrador, quiero recibir alertas de gas, para evitar emergencias. | 5 |
| 18        | US018          | Notificación en tiempo real               | Como huésped, quiero recibir notificaciones de seguridad, para sentirme protegido. | 3 |
| 19        | US019          | Registro histórico de alertas             | Como administrador, quiero consultar historial de alertas, para tener trazabilidad. | 3 |
| 20        | US020          | Integración de alertas con tareas de staff| Como administrador, quiero que alertas IoT generen tareas automáticas, para acelerar la respuesta. | 5 |
| 21        | US021          | Página inicial de la landing page         | Como visitante, quiero ver la página inicial, para obtener una visión general del sistema. | 2 |
| 22        | US022          | Sección de características de la landing  | Como visitante, quiero ver las características del sistema, para entender sus beneficios. | 2 |
| 23        | US023          | Sección de contacto en la landing         | Como visitante, quiero enviar un mensaje desde la landing, para solicitar más información. | 3 |
| 24        | US024          | Sección de planes de la landing           | Como visitante, quiero ver los planes de suscripción, para conocer opciones de precios. | 2 |
| 25        | US025          | Llamada a la acción (CTA – Solicitar demo)| Como visitante, quiero tener un botón de "Solicitar Demo", para pedir una prueba del sistema. | 2 |
