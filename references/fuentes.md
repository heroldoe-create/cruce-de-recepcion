# Fuentes y decisiones del cruce de recepción

Consulta documental realizada el **2026-10-29 (UTC)**. Son fuentes informativas oficiales,
no resultados de validación de los RFC/UUID ficticios del ejemplo. No se reproducen listados
con datos de contribuyentes. Las instrucciones fiscales se limitan a orientar la consulta,
conservar el resultado y remitir su interpretación al contador.

| ID | Autor y documento | URL | Consulta | Alcance utilizado |
|---|---|---|---|---|
| F1 | SAT — Verifica tus facturas | https://wwwmat.sat.gob.mx/aplicacion/80523/verifica-tus-facturas-electronicas | 2026-10-29 | Consulta sin autenticación con folio fiscal y RFC emisor/receptor, código de imagen y resultado imprimible; contempla comprobante no encontrado |
| F1a | SAT — Aplicación de verificación, enlazada por F1 | https://verificacfdi.facturaelectronica.sat.gob.mx/ | Intento 2026-10-29 | Portal para el usuario; el intento de apertura desde esta corrida devolvió «Timeout fetching». No se realizó ninguna consulta de comprobantes |
| F2 | SAT — Datos abiertos, contribuyentes publicados | https://www.sat.gob.mx/minisitio/DatosAbiertos/contribuyentes_publicados.html | 2026-10-29 | Sección específica 69-B con listado completo y categorías presuntos, definitivos, desvirtuados y sentencias favorables; 69 y 69-B Bis aparecen separados. La página indicaba "Información actualizada al 30 de septiembre de 2026" el 2026-10-29 |
| F3 | SAT — Consulta la relación de contribuyentes que realizan operaciones inexistentes | https://wwwmat.sat.gob.mx/consultas/76675/consulta-la-relacion-de-contribuyentes-que-realizan-operaciones-inexistentes | 2026-10-29 | Consulta por RFC o nombre completos; información que puede cambiar; listado completo e interpretación de definitivos que requiere intervención del contador |
| F4 | SAT — Formato de Factura (Anexo 20), preguntas sobre tipos de comprobante | https://wwwmatnp.sat.gob.mx/consultas/35025/formato-de-factura-electronica-(anexo-20) | 2026-10-29 | Catálogo de tipos I (ingreso), E (egreso), P (pago) y trazabilidad de notas de crédito hacia el comprobante de ingreso |

## Correspondencia con las reglas

- F1 respalda el procedimiento de consulta y la separación entre resultado aportado y factura
  leída. La skill registra el estado devuelto, sin certificar firmas ni efectos fiscales.
- F2 respalda conservar la categoría 69-B en vez de reducirla a «coincide/no coincide» y evitar
  confundirla con otros listados. La evidencia que aporte el usuario debe incluir su fecha.
- F3 respalda pedir identidad completa y fuente fechada. La skill no calcula plazos de defensa,
  no decide efectos fiscales ni califica al proveedor como fraudulento. El contador revisa la
  situación concreta y la norma vigente antes de decidir.
- F4 respalda distinguir tipos I/E/P y no confundir una nota de crédito o un comprobante de
  pago con una recepción de mercancía. La aplicación comercial de créditos requiere evidencia.
- La consulta fiscal que se adjunte corresponde a la fecha de la evidencia, no a una garantía
  permanente. No se adopta una supuesta vigencia legal de 72 horas.

## Reglas comerciales propias (no disposiciones fiscales)

El empate por OC/renglón/unidad, corte de recepciones, separación de daño, no duplicación de
UUID y fórmula B−C = Q+P son decisiones de diseño de este paquete. No son una exigencia del SAT.
No autorizan retener pagos ni modificar contratos. Las tolerancias, aceptación, devoluciones,
notas de crédito y fechas de respuesta dependen de la documentación del usuario.

El precio de referencia, el tratamiento de parciales y las cantidades del ejemplo son
convenciones comerciales explícitas, no reglas tributarias. No se incluye ninguna regla aduanal.
