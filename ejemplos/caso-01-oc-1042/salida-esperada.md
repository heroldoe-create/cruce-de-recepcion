## Matriz de cruce

**EJERCICIO FICTICIO — Andén Norte. Corte: 2026-10-29. MXN antes de impuestos.**
Fuentes: resúmenes de CFDI; no se aportaron XML originales. OC-1042 sin cambios ni tolerancias,
entrada completa REC-551 aplicada solo a F-8821 y condiciones en `verificacion-fiscal.txt`.
O = pedido, F = facturado, R = bueno aceptado; A = menor de O/F/R. Unidad: caja por SKU.

| SKU / renglón F-8821 | O | F | R | Daño rechazado | A | Po | Pf | B facturada | C referencia | B−C | Evidencia |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|---|
| AN-MZ-001 / 1 | 100 | 100 | 96 | 0 | 96 | 185.00 | 185.00 | 18,500.00 | 17,760.00 | 740.00 | OC-1042 r1; REC-551 r1; F-8821 r1 |
| AN-PL-002 / 2 | 50 | 55 | 55 | 0 | 50 | 120.00 | 120.00 | 6,600.00 | 6,000.00 | 600.00 | OC-1042 r2; REC-551 r2; F-8821 r2 |
| AN-LE-003 / 3 | 80 | 80 | 78 | 2 | 78 | 62.50 | 65.00 | 5,200.00 | 4,875.00 | 325.00 | OC-1042 r3; REC-551 r3; F-8821 r3 |
| AN-UV-004 / 4 | Sin OC confirmado | 10 | 0 confirmado | 0 | 0 | No aplica | 200.00 | 2,000.00 | 0.00 | 2,000.00 | F-8821 r4; REC-551 r4; confirmación compras en verificación |
| **F-8821 total** | — | — | — | — | — | — | — | **32,300.00** | **28,635.00** | **3,665.00** | Subtotal declarado coincide |

F-8799: subtotal MXN 18,500.00, sin OC/recepción asignadas ni sustitución documentada;
fuera de esta matriz comercial. No consumir REC-551 por segunda vez.

## Cola de diferencias

Responsables sugeridos; plazo de respuesta por acordar. Importes comerciales en MXN antes de impuestos.

| ID | Prioridad / clase | Folio / renglón | Hecho | Importe | Evidencia | Acción / responsable | Condición de cierre |
|---|---|---|---|---:|---|---|---|
| D01 | Alta / CFDI-CANCELADO y DATOS | F-8799 / documento | Estado simulado Cancelado; fecha del CFDI 2026-10-18, anterior a la OC-1042 (2026-10-20); mismo SKU, cantidad y precio que F-8821 r1; sin aplicación ni vínculo de sustitución | 18,500.00 documental; excluido del reclamo | Resumen F-8799 y verificación simulada | Aclarar documento y eventual sustitución / cuentas por pagar y contador | Resultado identificable y vínculo/aplicación documentados |
| D02 | Comercial / SIN-OC | F-8821 / 4 | 10 cajas facturadas sin OC ni ingreso confirmados | 2,000.00 | F-8821 r4; REC-551 r4; confirmación compras | Pedir soporte o propuesta de corrección / compras | OC/autorización válida y recepción o corrección documentadas |
| D03 | Comercial / FALTANTE | F-8821 / 1 | 4 cajas no llegaron, 100 facturadas contra 96 aceptadas | 740.00 | OC r1; CFDI r1; REC-551 r1 | Solicitar aclaración de entrega o propuesta de ajuste / compras | Entrega acreditada o ajuste acordado y documentado |
| D04 | Comercial / EXCESO-OC | F-8821 / 2 | 55 facturadas y recibidas contra 50 pedidas | 600.00 | OC r2; CFDI r2; REC-551 r2 | Acordar aceptación comercial o devolución / compras y almacén | Autorización escrita o devolución/ajuste documentados |
| D05 | Comercial / PRECIO | F-8821 / 3 | +2.50 por caja sobre 78 comparables | 195.00 | OC r3; CFDI r3; REC-551 r3 | Pedir respeto a precio pactado / compras | Precio justificado o ajuste documentado |
| D06 | Comercial / DAÑO/RECHAZO | F-8821 / 3 | 2 de las 80 cajas físicas rechazadas por daño | 130.00 | REC-551 r3; CFDI r3 | Acordar reposición o disposición/ajuste / almacén y compras | Reposición aceptada o solución documentada |

Estado simulado F-8821: Vigente. Emisor: sin coincidencia exacta en 69-B en fuente/fecha
simuladas aportadas (actualización 2026-10-28; consulta 2026-10-29 09:00 UTC).
No es una consulta real ni una certificación del proveedor.

## Control de importes

| Concepto | MXN | Cuenta a mano |
|---|---:|---|
| B, subtotal F-8821 | 32,300.00 | 18,500 + 6,600 + 5,200 + 2,000 |
| C, referencia comercial | 28,635.00 | 96×185 + 50×120 + 78×62.50 |
| Q, porción de cantidad/sin OC | 3,470.00 | 4×185 + 5×120 + 2×65 + 10×200 |
| P, precio en cantidad comparable | 195.00 | 78×(65−62.50) |
| B−C = Q+P | **3,665.00** | 32,300−28,635 = 3,470+195 |
| F-8799, exposición documental separada | 18,500.00 | Sin sumar a las diferencias comerciales |

En lechuga, 130 por daño + 195 por precio = 325. No agregar además 80×2.50 = 200,
porque duplicaría la diferencia de precio en las 2 cajas ya valoradas a 65.
C no es pago autorizado. Impuestos/total fiscal no aportados: no calculados.
No hay créditos o devoluciones aplicados según las condiciones simuladas aportadas.

## Carta al proveedor

**Asunto: Solicitud de aclaración — OC-1042 / REC-551 / F-8821 y documento F-8799**

Al Proveedor ficticio de Andén Norte:

Al cruzar su factura F-8821 con la OC-1042 y la recepción REC-551 del 26 de octubre de 2026,
identificamos las siguientes diferencias, en MXN antes de impuestos:

| Referencia | Diferencia | Importe por aclarar | Solicitud |
|---|---|---:|---|
| D02 / AN-UV-004 | 10 cajas facturadas sin OC autorizada ni ingreso | 2,000.00 | Aportar soporte de autorización/entrega o propuesta de corrección |
| D03 / AN-MZ-001 | 4 cajas faltantes | 740.00 | Aclarar entrega pendiente o proponer ajuste |
| D04 / AN-PL-002 | 5 cajas sobre lo pedido | 600.00 | Acordar aceptación comercial o devolución |
| D05 / AN-LE-003 | Precio de 65.00 frente a 62.50 en 78 cajas comparables | 195.00 | Justificar precio o proponer ajuste |
| D06 / AN-LE-003 | 2 cajas rechazadas por daño | 130.00 | Acordar reposición o disposición/ajuste |
| **Total comercial por aclarar** | | **3,665.00** | |

Adicionalmente, en este ejercicio el resultado aportado para F-8799 indica Cancelado.
Solicitamos aclarar su aplicación y, si existe, el vínculo con el documento vigente que lo
sustituye. Su subtotal de 18,500.00 se trata aparte y no integra el importe comercial anterior.

Solicitamos respuesta con el soporte de cada punto. Plazo de respuesta: por acordar.
Esta solicitud no confirma un saldo ni compromete una fecha de pago.

Cuentas por pagar de Andén Norte

## Pendientes y evidencia interna

| Dato / soporte | Responsable sugerido | Próximo paso |
|---|---|---|
| XML originales e impuestos/totales fiscales de ambas facturas | Cuentas por pagar | Aportar documentos originales; mantener el cruce limitado a resúmenes/subtotal |
| Aplicación y posible sustitución de F-8799 | Proveedor / contador | Confirmar historial, sin imputar otra vez REC-551 |
| Respuesta D02–D06 y plazo | Compras / proveedor | Acordar solución y conservar soporte |
| Disposición de 2 cajas dañadas | Almacén / compras | Documentar solución sin descontarlas otra vez como devolución |

Archivos consultados: `orden-compra.csv`, `recepcion-almacen.csv`,
`cfdi-f8821-resumen.csv`, `cfdi-f8799-resumen.csv`, `verificacion-fiscal.txt`.
El acta está descrita en la entrada del ejercicio; no se adjuntaron fotos ni acta firmada separada.
Consultas fiscales reales: no realizadas; todos los resultados son simulados.

Pre-revisión; no sustituye al contador, al agente aduanal ni al SAT. No autoriza pagos.
Basado en una skill de Heroldo Escobedo — heroldo.org
