# Aplicación nativa, productos y posventa — requisitos Matterssmith Commerce

**Estado:** planificación; no confundir con código ya implementado. Fecha: 2026-11-19.
**Requisitos heredados:** MAT-COM-003,007,008,010,013,018.
**Documento normativo:** https://github.com/Matterssmith/Marketplace-Matter/blob/matter/docs/REQUISITOS_ECOSISTEMA_COMERCIO.md.

## Necesidades de aplicación

1. **Acceso sin cuenta civil:** permitir explorar productos e información de garantías como invitado, con seguridad y limitaciones del dispositivo anfitrión.
2. **Alta de unidad Matter opcional:** vincular serie y comprobante de compra mediante desafío autorizado; pedir confirmación real antes de transferir al nuevo propietario. QR/NFC nunca debe contener información privada de cliente.
3. **Estado de propiedad:** mostrar únicamente `titularidad comprobada`, `garantía válida`, `servicio elegible` recibidos de Vault y autorización vigente.
4. **Reparaciones:** permitir solicitud, consentimiento de diagnóstico, registro de servicio, evidencia de entrega y disputa; técnicos y piezas se asocian al expediente. Los derechos legales siguen aplicándose aunque no haya registro.
5. **Puente nativo a dispositivo:** toda acción de Wi-Fi/Bluetooth/archivos/telemetría depende de permiso OS, propiedad y acción concreta. Compra de un aparato NO concede control silencioso de sus datos.
6. **Experiencia móvil:** catálogo y vídeos accesibles, estado de pedido, entrega y actualización autorizada; avisos sin localización precisa por defecto.
7. **Sin biometría obligatoria:** verificación de país y edad no son requisitos generales; un programa futuro de identidad se ejecuta por vía segura y consentimiento separado.

## Criterios de aceptación

- Registro de un serial duplicado falla, revocación elimina acceso de usuario anterior y todo cambio queda auditado.
- Invitado abre catálogo sin Vault. Acceso a datos de propiedad requiere autorización y falla cerrado si Vault no responde.
- Sin permiso OS / propietario, la aplicación no controla el hardware.
- Pruebas de cambio de dueño, robo reportado, reparación y acceso de técnico con datos ficticios.
- No se despliega app comercial ni control nativo por este commit; es documentación.

## Dependencias e instrucciones de trabajo

- Mantener contratos compatibles con Marketplace-Matter, Vault-Matter y API-Matter, sin almacenar copias de roles ni expedientes civiles.
- Antes de desarrollar: revisar privacidad, catálogo físico vs marketplace de software, escenarios de error y límites de acceso invitado.
- Por cada cambio registrar ticket/ID MAT-COM, responsable, tests, riesgo, aceptación y estado `proposed|approved|implemented|verified`.
- No habilitar pagos/entrega/reparaciones ni prometer generador validado sin la aprobación del responsable comercial y técnico.
- Bot-Matter sigue bloqueado; no convertir una UI o menú en autorización.

Créditos:
Hecho por Lournyx Matterssmith [Lou-Nyx].
