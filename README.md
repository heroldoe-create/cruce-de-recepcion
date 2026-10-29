# Cruce de recepción

CFDI del proveedor + consulta SAT/69-B hecha por ti + orden de compra + entrada física →
matriz trazable, cola de diferencias con responsables y carta al proveedor lista para copiar.
**Licencia para empresa: USD 20.** Autor: Heroldo Escobedo — heroldo.org.

## Uso en 3 pasos

1. Conecta la skill mediante el conector de Agensi en claude.ai, si lo tienes habilitado, o
   sube **cruce-de-recepcion.zip** desde la opción de cargar skills de tu cuenta. La disponibilidad
   de esas opciones depende de tu cuenta; el ZIP también contiene el texto de la skill.
2. Adjunta o pega tu CFDI (XML o PDF), orden de compra y recepción (Excel, CSV, foto legible
   o texto). Pide: **«Cruza estos documentos. Dame la matriz, la cola y la carta al proveedor»**.
   Puedes indicar corte, tolerancias y plazo acordados; no necesitas preparar una plantilla.
3. En tu validador habitual consulta cada UUID y el RFC del emisor en **69-B**; la skill te
   indica qué copiar. Pega el resultado con fuente y fecha, incluida categoría y actualización
   del listado. Recibe los documentos listos; si falta algo, el cruce comercial sale con una
   tabla breve de pendientes. Revisa la carta y envíala tú.

Sin terminal, scripts obligatorios, API ni configuración técnica. No necesita acceso a tu sistema
administrativo. No adjuntes contraseñas, certificados privados ni llaves.

## Qué recibes

- Matriz con cantidades pedidas, facturadas, buenas y dañadas, precios y origen de cada cifra.
- Cola por prioridad: incidencias fiscales/documentales, faltantes, daños, exceso, precios y
  mercancía sin orden; con importe o «no calculable», responsable y condición de cierre.
- Control de importes sin sumar dos veces la misma diferencia; impuestos separados.
- Carta comercial y pendientes internos listos para copiar, sin introducciones.

Acepta entregas parciales y múltiples documentos cuando su aplicación está documentada. Si no
hay equivalencias, vínculo entre entregas/facturas o evidencia fiscal, lo marca; no adivina.
**No sustituye al contador, al agente aduanal ni al SAT:** pre-revisa, cruza y arma evidencia.
No valida firmas ni timbra, no decide deducciones ni pagos y no manda mensajes.

## Prueba sin datos propios

Escribe en el chat: **«Corre el ejemplo incluido de la skill cruce-de-recepcion»**. Si tu forma de instalación no
trae los archivos, ábrelos del ZIP (carpeta `ejemplos/caso-01-oc-1042/`) y adjunta los cinco de entrada (todos menos
`salida-esperada.md`) con la frase del paso 2. Compara con
`salida-esperada.md`: **MXN 32,300.00 − 28,635.00 = 3,665.00**, antes de impuestos.
La factura cancelada se informa aparte, sin sumarla al reclamo. Todo es **FICTICIO de Andén
Norte**, incluidos RFC, UUID y resultados fiscales; no representa consultas al SAT.
`ejemplos/casos-limite.md` contiene comprobaciones adicionales a mano.

## Contenido

`skills/cruce-de-recepcion/SKILL.md` contiene las instrucciones de autoría;
`references/fuentes.md`, las fuentes oficiales con fecha de consulta;
`ejemplos/`, entradas y resultados reproducibles; `LICENSE`, la licencia completa.
`cruce-de-recepcion.zip` lleva una carpeta `cruce-de-recepcion/` con SKILL.md directamente en
su raíz, referencias, ejemplos, README y LICENSE, para cargarla sin reorganizar archivos.
El paquete no depende de rutas privadas, de otras skills ni de herramientas del autor.


## Licencia

**Propiedad intelectual de Heroldo Escobedo**, con el código a la vista ([Licencia de uso de Heroldo 1.0](LICENSE)):

- **Uso personal: gratis.** Léelo, pruébalo y adáptalo para aprender o en tus propios datos.
- **Uso en una empresa o con fines de lucro: solo con compra.** Cómpralo en [Agensi](https://agensi.io/skills/cruce-de-recepcion)
  o escribe a heroldo@lolo-enterprises.com. La compra cubre a tu empresa.
- **Siempre se cita la fuente:** «Basado en una skill de Heroldo Escobedo — heroldo.org».
- No se revende ni se vuelve a publicar.

> **In English:** Source-available, not open source. Free for personal use. Business use requires purchase on
> [Agensi](https://agensi.io/skills/cruce-de-recepcion). Attribution to Heroldo Escobedo — heroldo.org is always required.
