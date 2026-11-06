# TPI-Organizaci-nEmpresarial-ProyectoSTOED-McDonald-s-DiazJulianIsmael
Proyecto STOED para el TPI de Organización Empresarial. Enfocado en McDonald's como organización.

## Datos Institucionales
* **Institución:** Universidad Tecnológica Nacional (UTN)
* **Carrera:** Tecnicatura Universitaria en Programación a Distancia (TUP AD)
* **Materia:** Organización Empresarial
* **Cuatrimestre - Año:** 2° Cuatrimestre - 2026
* **Docentes:**
    * Prof. Titular: Dra. Gabriela Martínez
    * Prof. Adjuntos: Carolina Bruno, Mario Raúl López, Andrea Ramos
* **Alumno:** Julian Ismael Diaz


---



## Descripción del Proyecto
El **Módulo STOED** (*Sistema de Trazabilidad Operativa y Estimación Dinámica*) esta pensado
como una solución para UNA sucursal piloto (de prueba) que tenga un medio-alto tráfico
de McDonald's. La idea es entregar un MVP (Producto Minimo Viable) para el testeo.

El objetivo principal del Módulo es estimar y mostrar en tiempo real los tiempos de 
preparación y entrega de pedidos en Salón(el propio local), AutoMac y Delivery (sea la app que sea), coordinando la demanda con el inventario y las estaciones de cocina KVS (*Kitchen Video System*).


---


## Metas Cuantitativas del Sistema (KPIs)
1. **Precisión de Estimación:** El margen de error debe ser menor o como mucho iugal al
10% en el, por lo menos, 90% de los pedidos que sean procesados.
2. **Latencia del Servidor:** El tiempo de respuesta ideal del servidor debe ser menor a 
1,5 seg aprox.
3. **Capacidad de Concurrencia:** Sostener hasta, aprox 500 pedidos a la vez en hora pico.
4. **Plazo de Ejecución:** Ciclo completo de desarrollo en 16 semanas, como estimación.


---


## Estructura del Proyecto y Entidades de Datos
El sistema se soporta en 4 entidades del negocio:
* `PEDIDO`: este registra el canal de origen, las transacciones y el tiempo estimado en segundos.
* `ESTADO_TRAZABILIDAD`: monitor de los hitos de cocina ('Recibido', 'Cocción'. 'Empaquetado', 'Listo').
* `PRODUCTO_MENU`: clave para administrar los tiempos estándar y la disponibilidad de stock
en cocina.
* `REPARTIDOR_DELIVERY`: para capturar coordenadas GPS e integrar los tiempos de arribo de 
plataformas externas como Rappi o PedidosYa.


---


## Historia de Usuario (Backlog del Proyecto)
* **HU01 (Cliente - App Mobile):** **Como** cliente de McDonald's, **quiero** visualizar en tiempo real la estimación dinámica de preparación de mi pedido, **para** organizar mi llegada a la sucursal o recepcionar sin demoras innecesarias.
* **Estado en Kanban:** `Listo` (*Done*)

* **HU02 (Personal de Cocina - KVS):** **Como** trabajador en la cocina, **quiero** ir registrando  y actualizar estado de las comandas directamente en la pantalla táctil KVS, **para** nuestro orden y la calma del público.
* **Estado en Kanban:** `En Progreso` (*In Progress*)

* **HU03 (Repartidor - Delivery):** **Como** repartidor, **quiero** sincronizar mi ubicación GPS con la sucursal, **para** poder llegar a tiempo justo cuando lo terminan de preparar, asi no se enfría la comida.
* **Estado en Kanban:** `Por Hacer` (*To Do*)


---


## Declaración de Transparencia sobre el uso de IA
En cumplimiento de las pautas de la cátedra, declaro el uso de asistentes bajo las siguientes condiciones:
* **Prompts para la IA:** En general, para cada parte del TPI asi como la unión de los mismos, le pedí siempre ideas sobretodo, sea esquemas, gráficos así como los contenidos para su posterior revisión y corrección por respuesta.

**EJEMPLO DE PROMPT:**
“Interdependencia de Módulos: Proponer un área o módulo de software específico que requiera desarrollo o mejora (ej. comercialización, inventario, facturación) y explicar detalladamente cómo su implantación alterará e interactuará sistémicamente con las demás dependencias de la organización. 
se me ocurre algo relacionado con el inventario y los recursos del local, por ejemplo un software que pueda calcular el tiempo estimado de espera para el local, para el automc y para el delivery tambien, con el mayor seguimiento posible e incluso algo visual como (estan preparando tu hamburguesa, añadiendo aderezos, empaquetando tu pedido, en camino -> si es delivery que siga mediante ubicacion) todo que se pueda ver desde la app y pantallas en el local en el caso de estar presencial“

Luego de eso fuimos corrigiendo y consolidando para que se adapte la idea a McDonald’s y como debía ser según los requerimientos y contenidos de la cátedra.

* **Propósito de uso:** Para corregir el estilo, sea ortográfico como del diseño, sumado a una guía de como estructurar, en este caso los diagramas BPMN y el formato Markdown de la documentación técnica.
* **Control Crítico Humano:** Todos los conceptos y respuestas, asi como diagramas y demás, son revisados antes de la previa entrega.
* **Responsabilidad Intelectual:** Asumo como estudiante la autoría integral y la responsabilidad técnica total sobre el proyecto.

**La revisión del PR fue realizada por el propio autor por tratarse de un trabajo individual; los comentarios y correcciones quedan documentados en el PR**
---


## Enlaces Importantes
* **Tablero de Gestión Ágil (GHithub Projects/Jira):** https://github.com/users/julianidiaz98/projects/4/views/1
* **Documentación PDF Integradora Final:** Disponible en la raíz del repo(`TPI_FINAL_OrganizacionEmpresarial_DIAZ.pdf`).
