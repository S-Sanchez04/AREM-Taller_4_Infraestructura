# 📄 Informe Técnico del Taller

## 🔖 Nombre del Taller
_Taller 4 - Mapa de Infraestructura de Macondo Magic Softwares_

## 👥 Integrantes del equipo
- Santiago Sánchez Cárdenas
- Mateo Gonzalez Cano

## 🧠 Descripción general del trabajo
El objetivo del taller fue modelar un mapa de infraestructura que reflejara de manera realista el ecosistema tecnológico actual de la empresa Macondo Magic Softwares. Para ello se identificaron los principales actores, herramientas y plataformas utilizadas en la gestión de proyectos, comunicación interna y entrega de software.

## 🔧 Proceso de desarrollo
El trabajo se desarrolló a partir de un levantamiento inicial de supuestos: Macondo no cuenta con un ERP ni con infraestructura propia compleja, sino que combina servicios en la nube con herramientas de productividad comunes (Office, WhatsApp, correo). Se priorizó modelar un flujo desde la recolección de requerimientos hasta la entrega final de los productos, pasando por gestión, desarrollo y despliegue.

Primero se definieron los bloques clave (usuarios, requerimientos, gestión, comunicación, desarrollo, despliegue). Posteriormente se identificaron herramientas como: Word/OneDrive para documentación, Jira para gestión de proyectos, Git para control de versiones y Alibaba Cloud para despliegue. Finalmente se construyó el diagrama en Draw.io.

## 🧩 Análisis del modelo propuesto
El modelo se estructura de forma secuencial desde la interacción de clientes (usuarios) hasta la entrega final de los productos de software. Representa las necesidades del cliente porque:
- Incluye canales de comunicación directa (correo, WhatsApp).
- Considera herramientas simples de requerimientos (Word/OneDrive).
- Integra plataformas técnicas mínimas para desarrollo y despliegue (Git, nube).

Se identificó que Macondo no posee servidores locales ni herramientas avanzadas para los flujos en el bussiness.

## 📈 Diagrama final entregado
![Mapa de Infraestructura de Macondo](Diagrama%20de%20Infraestructura%20Macondo.drawio.png)

[📄 Versión PDF](./Diagrama%20de%20Infraestructura%20Macondo.drawio.pdf) 

## 📋 Tabla de actores, entidades o componentes (si aplica)

| Nombre del elemento | Tipo             | Descripción                                                                 | Responsable              |
|---------------------|------------------|-----------------------------------------------------------------------------|--------------------------|
| Clientes            | Actor externo    | Usuarios que acceden a la web de Macondo Softwares a través de Internet.    | Externo (Usuarios)       |
| Dominio (DNS)       | Infraestructura  | Servicio DNS que traduce `macondosoftwares.com` a una dirección IP.         | Proveedor de DNS / TI    |
| Load Balancer       | Infraestructura  | Distribuye el tráfico de clientes hacia el servidor web (WordPress).        | Área TI / Proveedor nube |
| Firewall            | Seguridad        | Filtra el tráfico entre la zona pública, DMZ y privada.                     | Área TI / Seguridad      |
| App Web (WordPress) | Aplicación       | Sitio web corporativo para interacción con clientes y formularios.          | Área Web / Marketing TI  |
| Base de Datos       | Datos / Infra    | Almacena la información del sitio web (usuarios, formularios, contenido).   | Área TI                  |
| Backups de Data     | Infraestructura  | Sistema de respaldo periódico de la base de datos y archivos del sitio.     | Área TI                  |
| Logs                | Datos / Seguridad| Registros de actividad y auditoría del sistema para monitoreo y análisis.   | Área TI / Seguridad      |


## 🔍 Investigación complementaria
### Tema investigado:
Buenas prácticas en la modelación de infraestructura con C4.

### Resumen:
El modelo C4 propone representar la infraestructura tecnológica en distintos niveles de detalle (contexto, contenedores, componentes, código). Para este taller se trabajó principalmente en un nivel de contenedores, mostrando aplicaciones y servicios relevantes sin entrar en la configuración detallada de servidores. Este enfoque permite comunicar de manera clara cómo fluye la información entre actores, herramientas y plataformas.

La aplicación de C4 a un caso como Macondo muestra que es posible simplificar la notación sin perder relevancia: se representaron tanto los recursos ofimáticos (Word/OneDrive) como los servicios técnicos mínimos (Git, nube), logrando un balance entre realismo y claridad.

## 📚 Referencias
- [1] Brown, Simon. *The C4 Model for Software Architecture*. https://c4model.com
- [2] Universidad de La Sabana. Material del curso AREM - Arquitectura Empresarial.

---

_Este documento hace parte de la entrega del taller 4 del curso AREM (Arquitectura Empresarial) - Universidad de La Sabana._
