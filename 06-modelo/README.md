# Modelo financiero y valuación

`Modelo_Satrack_Fase4.xlsx` — proyección de P&L a 5 años, calendario de deuda,
valuación de entrada y salida, y puente de retorno, todo con fórmulas activas: al
cambiar cualquier supuesto en amarillo, el resto del archivo se recalcula.

## Estructura del archivo

- **Instrucciones** — cómo usar el archivo y de dónde sale cada dato base.
- **Supuestos** — todas las celdas editables: TRM, crecimiento, márgenes, estructura
  de capital, múltiplos de entrada y salida.
- **Proyección P&L** — ventas, EBITDA y utilidad neta, 2025 a 2030.
- **Deuda** — calendario de deuda a 5 años con amortización lineal.
- **Valuación y Retorno** — EV de entrada y salida, ticket de equity, MoM, IRR, y
  una tabla de sensibilidad 3x3 (múltiplo de entrada x múltiplo de salida).
- **Puente de Retorno** — descompone la creación de valor en crecimiento de
  EBITDA, expansión de múltiplo y desapalancamiento.

## Punto de partida y supuestos clave

| Supuesto | Valor | De dónde sale |
|---|---|---|
| TRM | 3,192 COP/USD | Tipo de cambio del día del análisis |
| Ventas 2025 | US$32.2M | SIIS, corte 2025-12-31 |
| EBITDA 2025 | 17.35% margen | EBIT + D&A real, vía flujo de efectivo de SIIS |
| Crecimiento orgánico anual | 13% | CAGR observado 2024-2025 de la propia empresa |
| Boost por add-ons (años 2-4) | +5% | Supuesto — roll-up de competidores, mismo patrón que Numaris |
| Expansión de margen EBITDA anual | 0.8pp | Apalancamiento operativo ya observado (margen EBIT subió 3.5pp en un año) |
| Múltiplo de entrada | 6.0x-8.0x (base 7.0x) | Supuesto razonado — sin comparable de transacción confirmado en el sector |
| Múltiplo de salida | 7.5x-9.5x (base 8.5x) | Supuesto razonado |
| Deuda / EBITDA al cierre | 1.0x | Conservador, coherente con el estilo de underwriting declarado de Linzor |

**Ninguno de los múltiplos de valuación está verificado contra una transacción
comparable confirmada del sector.** El único precedente cualitativo de cómo Linzor
estructura un deal de control en Colombia es Onest Colombia (2015, aumento de
capital de US$39M, sector de crédito especializado, con el Fondo III) — se usa como
evidencia del patrón de estructuración, no como ancla numérica de múltiplo.

## Resultado del caso base

| | |
|---|---|
| Ticket de equity Linzor (entrada) | US$26.9M |
| Proceeds a Linzor (salida, año 5) | US$98.2M |
| MoM | 3.66x |
| IRR | 29.6% |

El ticket cae dentro del rango de pólvora seca estimado para el Fondo IV de Linzor
(US$15-40M, ver `../01-research-linzor/`). El puente de retorno muestra que el
69% del valor creado viene de crecimiento de EBITDA, 24% de expansión de múltiplo, y
solo 6% de desapalancamiento — coherente con el estilo de creación de valor
operacional, no financiero, que Linzor declara públicamente.
