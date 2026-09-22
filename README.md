# Reto Linzor — Caso de inversión: Satrack S.A.S.

Manuel De la Tejera González · [manuel.delatejerag@gmail.com](mailto:manuel.delatejerag@gmail.com)

Este repositorio documenta el proceso completo detrás de mi propuesta para el Reto
Linzor: identificar una empresa en México o Colombia con ventas anuales sobre
~US$10 millones, evaluarla como potencial inversión de Linzor Capital Partners, y
construir el caso en 3 slides.

No incluyo solo la conclusión — incluyo cómo llegué a ella, qué descarté y por qué, y
qué preguntas dejé abiertas. Mi intención fue seguir el mismo proceso que seguiría un
analista de PE: entender primero el mandato del fondo, construir un embudo de
candidatos con criterio explícito, y solo después bajar a un modelo y una tesis.

## La conclusión, en una página

**Target: Satrack S.A.S.** (Medellín, Colombia) — telemática y gestión de flotas,
fundada en 1994, liderada por Federico Salazar Pineda desde el año 2000. Es una réplica
directa, en un segundo mercado del portafolio de Linzor, de la tesis que el fondo ya
validó con Numaris en México: SaaS de flotas en un sector fragmentado, maduro para
consolidación por adquisiciones.

| | |
|---|---|
| Ventas 2025 | US$32.2M |
| Margen EBITDA | 17.4% |
| Crecimiento interanual | +12.8% |
| Ticket de equity estimado | US$26.9M |
| MoM a 5 años (caso base) | 3.66x |
| IRR (caso base) | 29.6% |

**El argumento central:** los fondos globales ya se llevaron los mejores activos de
software colombianos visibles — Advent International compró Siesa en diciembre de
2024, H.I.G. Capital compró Digital Ware en 2019. Satrack cae exactamente en la
ventana de tamaño que esos fondos ya no pueden tocar (muy pequeña para su ticket
mínimo) y que el capital de riesgo tampoco alcanza (muy madura, sin narrativa de
hipercrecimiento). Es el hueco que el Fondo IV de Linzor — más chico que sus
predecesores, con ~US$60-80M de pólvora seca restante — sí puede llenar.

**[Las 3 slides finales están en `05-pitch/`](./05-pitch/)**, junto con el código
fuente y las notas de cómo defender cada afirmación en vivo.

## Cómo se construyó este caso

El proceso siguió seis fases, y cada carpeta corresponde a una:

1. **[`01-research-linzor/`](./01-research-linzor/)** — Antes de buscar una empresa,
   entendí qué busca Linzor: tamaño de fondo, temas de inversión declarados, patrones
   repetidos en su portafolio, y un hueco identificable en su estrategia (nunca han
   originado una plataforma de software en Colombia).
2. **[`02-screening/`](./02-screening/)** — Un embudo top-down de 33 empresas
   colombianas, filtradas por tamaño, sector y disponibilidad de datos públicos, con
   una matriz de scoring ponderado.
3. **[`03-target-satrack/`](./03-target-satrack/)** — Deep dive del target elegido:
   perfil de negocio, análisis financiero completo (Superintendencia de Sociedades),
   y lo que pude —y no pude— confirmar sobre su propiedad y ángulo de transacción.
4. **[`03-target-satrack-backup-sincosoft/`](./03-target-satrack-backup-sincosoft/)**
   — El target de respaldo, documentado por si la verificación de Satrack hubiera
   fallado.
5. **[`04-memo/`](./04-memo/)** — El memo de decisión que comparó ambos targets y
   explica por qué Satrack ganó, pese a que Sincosoft es el mejor negocio en varios
   criterios fundamentales.
6. **[`06-modelo/`](./06-modelo/)** — El modelo financiero de 5 años: proyección de
   P&L, calendario de deuda, valuación de entrada y salida, y el puente de retorno
   que sustenta el MoM y el IRR reportados arriba.

## Lo que reconozco que no logré cerrar

Prefiero dejar esto explícito en vez de que parezca que se me pasó:

- **No confirmé formalmente, vía Cámara de Comercio de Medellín, si Federico Salazar
  Pineda es también el representante legal registrado de Satrack.** El portal RUES
  presentó fallas de acceso repetidas durante la investigación. La evidencia que sí
  tengo —26 años como "President" según su propio perfil de LinkedIn, tras haber
  liderado el desarrollo del producto original desde 1996— es sólida pero no
  notarial. Detalle completo en
  [`03-target-satrack/03-propiedad-angulo-transaccion.md`](./03-target-satrack/03-propiedad-angulo-transaccion.md).
- **El salto del pasivo por impuestos corrientes de Satrack en 2025 (~20x interanual)
  no lo investigué a fondo** — queda como pregunta abierta para una diligencia formal.
- **Los supuestos de crecimiento, margen y múltiplos del modelo financiero son
  razonados a partir de la trayectoria observada de la propia empresa, no verificados
  contra comparables de transacción confirmados en el sector.** El único precedente
  con cifra pública de cómo estructura Linzor un deal de control en Colombia es Onest
  Colombia (2015), y es de un sector distinto (crédito especializado, no software).

## Fuentes

- SIIS — Sistema Integrado de Información Societaria, Superintendencia de Sociedades
  de Colombia (siis.ia.supersociedades.gov.co)
- linzorcapital.com — portafolio, tesis de inversión declarada, comunicados de prensa
- LinkedIn — perfiles y páginas de empresa, consultados manualmente
- Prensa económica colombiana (Portafolio, La República, Valora Analitik, Forbes
  Colombia)
