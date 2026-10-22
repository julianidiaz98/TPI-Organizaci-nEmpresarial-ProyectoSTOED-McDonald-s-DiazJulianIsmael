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
* **HU01 (Cliente - App Mobile):** *Como cliente, me gustaría ver en la App el tiempo estimado de preparación, para coordinar cuando tenga que retirarlo o recibirlo en caso de.*
* **HU02 (Personal de Cocina - KVS):** *Como trabajador en la cocina, me parece correcto ir registrando el avance de las etapas en la pantalla KVS, para nuestro orden y la calma del público.*
* **HU03 (Repartidor - Delivery):** *Como repartidor, si sincronizo mi ubicación con la sucursal, podría llegar a tiempo justo cuando lo terminan de preparar, asi no se enfría la comida.*


---


## Declaración de Transparencia sobre el uso de IA
En cumplimiento de las pautas de la cátedra, declaro el uso de asistentes bajo las siguientes condiciones:
* **Propósito de uso:** Para corregir el estilo, sea ortográfico como del diseño, sumado a una guía de como estructurar, en este caso los diagramas BPMN y el formato Markdown de la documentación técnica.
* **Control Crítico Humano:** Todos los conceptos y respuestas, asi como diagramas y demás, son revisados antes de la previa entrega.
* **Responsabilidad Intelectual:** Asumo como estudiante la autoría integral y la responsabilidad técnica total sobre el proyecto.


---


## Enlaces Importantes
* **Tablero de Gestión Ágil (GHithub Projects/Jira):** https://github.com/users/julianidiaz98/projects/4/views/1
* **Documentación PDF Integradora Final:** Disponible en la raíz del repo(`TPI_FINAL_OrganizacionEmpresarial_DIAZ.pdf`).