   # OCI-001 - Evidencia de Cambio

   ## Cambio: Módulo de recaudo por QR - Corredor Urabá
   **Problema:** Filas en taquilla y pérdida de bus en Apartadó-Carepa-Turbo-Necoclí

   **Solución:**
   - api-venta-boletos: QrPagoStrategy para impresión 58mm/80mm
   - app-movil-inspector: Validación QR Offline-First
   - PostgreSQL: tabla pagos_qr + campo metodo_pago_id
   - Redis: Bloqueo pesimista anti-sobreventa

   **Trazabilidad GitHub:**
   Closes #1
   ACC: John Jiménez Moreno
   Fecha: 2026-10-04
