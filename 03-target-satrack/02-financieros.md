# Satrack — Análisis financiero

Fuente: SIIS (Superintendencia de Sociedades), corte 2025-12-31, "Pymes-Consolidados".
Todas las cifras en COP millones salvo que se indique otra unidad.

**Una limitación de los datos, declarada de entrada:** SIIS solo tiene tres cortes
disponibles para Satrack y su entidad histórica relacionada: 2025, 2017 y 2016. No
hay dato entre 2018 y 2023. La explicación más probable es que la empresa se
reestructuró como grupo consolidado en algún punto de ese rango, saliendo y
reentrando a la muestra de empresas vigiladas por Supersociedades — lo cual es, en sí
mismo, congruente con una empresa que ha estado creciendo.

## Estado de resultados

| | 2024 | 2025 | Variación |
|---|---|---|---|
| Ingresos | 91,207 | 102,903 | +12.8% |
| Ganancia bruta | 65,567 | 76,547 | |
| Margen bruto | 71.9% | 74.4% | ↑ |
| Ganancia operacional (EBIT) | 8,079 | 12,775 | +58.1% |
| Margen EBIT | 8.9% | 12.4% | ↑ fuerte |
| Ganancia neta | 6,138 | 9,158 | +49.2% |
| Margen neto | 6.7% | 8.9% | ↑ |

**EBITDA real**, no un proxy: el detalle del flujo de efectivo de SIIS muestra
depreciación y amortización de $5,081 millones en 2025. EBITDA = EBIT + D&A =
$17,856 millones, **margen EBITDA de 17.35%** (~US$4.46M a la TRM del momento del
análisis, y ~US$5.59M a la TRM más reciente usada en el modelo final — ver
`06-modelo/`).

**Una aparente contradicción que vale la pena explicar de antemano:** una fuente
externa (EMIS) reporta que el EBIT de Satrack cayó -18.2% en 2024, mientras que el
propio SIIS muestra que subió con fuerza (+58%) de 2024 a 2025. Ambos datos son
compatibles: sugieren que 2023 fue un año fuerte, 2024 uno flojo, y 2025 una
recuperación marcada — volatilidad año a año, no una tendencia de deterioro.

## Balance

| | 2024 | 2025 | Variación |
|---|---|---|---|
| Activos totales | 31,445 | 37,532 | +19.4% |
| Pasivos totales | 9,761 | 13,081 | +34.0% |
| Patrimonio total | 21,684 | 24,451 | +12.8% |

El pasivo creció casi tres veces más rápido que el patrimonio. El detalle: el pasivo
por impuestos corrientes se disparó de $48,811M a $982,168M (~20x) — una señal que no
alcancé a investigar a fondo y que dejo como pregunta abierta para diligencia
formal. El resto del crecimiento del pasivo corriente es, en cambio, cuentas por
pagar comerciales creciendo con el negocio, no deuda financiera alarmante (préstamos
corrientes: apenas $727M en 2025).

## Indicadores de solvencia y rentabilidad

| Indicador | Valor | Lectura |
|---|---|---|
| Prueba ácida | 2.06x | Liquidez sólida, sin depender de inventario |
| Endeudamiento | 34.85% | Moderado, financiado mayoritariamente con patrimonio |
| ROA | 24.4% | |
| ROE | 37.5% | ROE muy por encima de ROA confirma apalancamiento positivo |

## Flujo de efectivo (2025)

| | COP mm |
|---|---|
| Flujo operativo | +17,421 |
| Flujo de inversión | -4,569 |
| Flujo de financiación | -5,019 |
| — de los cuales, dividendos pagados | -5,158 |

El flujo operativo casi duplica la utilidad neta ($17,421M vs. $9,158M) — la utilidad
contable está respaldada por generación real de caja, no por cuentas por cobrar sin
cobrarse. Es la señal más tranquilizadora de todo el análisis financiero.

Los dividendos pagados ($5,158M, más de la mitad del EBITDA del año) confirman que
los accionistas extraen caja activamente del negocio. Decidí no usar este dato como
argumento de "ángulo de transacción" en la propuesta final — es un argumento de doble
filo: se puede leer igual de bien como "buscan liquidez y podrían abrirse a vender"
que como "ya tienen la liquidez que quieren sin ceder control". El razonamiento
completo de esa decisión está en [`05-pitch/`](../05-pitch/).

## Estado legal

"Procesos en Superintendencia: 0 activos, 0 cerrados". Sin banderas rojas legales
visibles en la fuente consultada.

## Conclusión

Satrack es una empresa financieramente sana y en mejora, no en deterioro. El bache
de EBIT de 2024 fue un año flojo dentro de una trayectoria más amplia de crecimiento,
no una tendencia. El único punto abierto de peso es entender la causa del salto del
pasivo por impuestos corrientes antes de comprometerse con cualquier valuación final.
