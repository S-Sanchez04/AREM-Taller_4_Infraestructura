# 🗒️ Registro de Trabajo en Clase - Taller 4

## 📆 Fecha de la sesión
_6/09/2025_

## 👥 Integrantes presentes
- Santiago Sánchez Cárdenas
- Mateo Gonzalez Cano

## 🧠 Actividades realizadas en clase

Durante la sesión se trabajó en el mapa de infraestructura del caso RedExpress, representado con notación inspirada en C4 (nivel contenedor):

- Se discutió la separación entre aplicaciones cliente (Plataforma Web y App móvil) y los servicios en la nube.  
- Se decidió representar la nube como un contenedor que agrupa: API Gateway, Load Balancer y Base de datos distribuida.  
- Se identificaron zonas críticas y posibles puntos de fallo:
  - Load Balancer → riesgo de sobrecarga si no se replica.  
  - DB distribuida → dependencia crítica para disponibilidad y consistencia.  
  - Módulo de procesamiento de rutas → componente central, cuello de botella potencial.  
  - Servidores regionales → pueden ralentizar la comunicación si no se escalan.  
- Se alcanzó a desarrollar el diagrama digital completo con actores, aplicaciones y nube.

## 🧩 Boceto inicial del modelo

![Mapa de infraestructura](Caso%20RedExpress.drawio.png)
[📄 Versión PDF](./Caso%20RedExpress.drawio.pdf) 

## 🔁 Tareas definidas para complementar el taller

| Tarea asignada | Responsable | Fecha estimada |
|----------------|-------------|----------------|
| Revisión y finalización del diagrama en draw.io | Santiago Sánchez Cárdenas | 10/09 |
| Redacción final del informe técnico | Mateo Gonzalez Cano | 13/09 |

---

_Este documento resume el trabajo colaborativo realizado durante la sesión del taller 4 en el curso AREM - Universidad de La Sabana._
