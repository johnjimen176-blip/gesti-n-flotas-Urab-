# Plataforma de Gestión de Flotas - Corredor Urabá (Apartadó - Carepa - Turbo - Necoclí)

## 1. Catálogo de Elementos de Configuración de Software (ECS/EGC)
| Clasificación | Elementos bajo control de configuración |
| :--- | :--- |
| **Programas** | Modulo Web de Ventas, App Android Inspector Offline-First, API Gateway (Nginx), Servicio Transaccional de Asientos. |
| **Datos** | Base de Datos PostgreSQL 16 (PostGIS), Clúster Redis (Bloqueos ACID). |
| **Documentación** | Documento de Diseño Arquitectónico (Event-Driven), Especificación Patrones State y Strategy, Manual Técnico de API. |

## 2. Plantilla de Solicitud de Cambio (Pull Request / Merge Request)
**Orden de Cambio de Ingeniería (OCI):** Implementación de módulo de pago electrónico (Código QR) en taquilla y app móvil.
**Justificación:** Reducir el recaudo en efectivo en los tramos rurales del Urabá.
**Análisis de Impacto Técnico:** 
- *Esfuerzo técnico:* Requiere integración de API bancaria en el API Gateway y actualización de la app Android.
- *Efectos secundarios:* Modifica el patrón Strategy de emisión de tiquetes para incluir el QR de pago.

## 3. Lista de Chequeo de Auditoría de Configuración
* **¿Qué cambió?** Se modificó el módulo de facturación y la estrategia de impresión.
* **¿Quién lo autorizó?** Autoridad de Control de Cambios (ACC) - Rol: Líder de Configuración.
* **¿Qué más se vio afectado?** El esquema de BD (PostgreSQL) requirió un nuevo campo.
* **¿Cuándo pasó?** Liberación de la versión v1.1.0.
