# Cómo construí el embudo de candidatos

## Por qué Colombia

Elegí Colombia sobre México por una razón práctica que también resultó ser
estratégica: la Superintendencia de Sociedades publica estados financieros de la
mayoría de las sociedades comerciales vigiladas del país, vía su plataforma SIIS —
algo sin equivalente directo en México. Eso hace posible construir un screening
cuantitativo real, no solo cualitativo.

La elección resultó reforzada por dos datos de contexto: Colombia estaba
subrepresentada en el portafolio de Linzor (solo un deal, Sies Salud), y fue el
mercado de M&A tecnológico más activo de la región en 2025 (software fue el sector
con más transacciones, 35 en el año).

## El filtro de screening

- Ventas anuales **sobre** ~US$10M — esto es un piso, no un rango objetivo. La
  propia convocatoria del Reto lo confirma con el símbolo ">" en su resumen:
  "Ventas > ~US$10mm".
- Ticket de equity implícito objetivo: US$15-40M, dado el tamaño del Fondo IV (ver
  `01-research-linzor/`).
- Sector primario: software vertical B2B / SaaS. Sector alternativo evaluado: salud
  de pago privado, como plan B si software no rendía candidatos limpios.
- Fundador operativo dispuesto a quedarse; algún ángulo de transacción identificable
  (sucesión, necesidad de capital para crecer, liquidez de accionistas).
- Mercado fragmentado, con adquisiciones potenciales identificables (para sostener
  una tesis de roll-up, como la de Numaris).
- Poca deuda; retorno esperado vía crecimiento de EBITDA y expansión de múltiplo, no
  apalancamiento.

## Subsectores que evalué

Consideré cinco subsectores antes de decidirme por software:

1. **Software vertical B2B** — el elegido, por ser réplica directa del patrón de
   Numaris.
2. **Salud de pago privado / adyacencia a Sies Salud** — plan B. La mayoría de las
   IPS pequeñas que investigué no reportan a Supersociedades (probablemente porque
   son fundaciones sin ánimo de lucro) o ya fueron adquiridas por consolidadores
   regionales.
3. Educación técnica — no lo profundicé más allá del screening inicial.
4. Crédito/leasing de nicho — descartado por ser demasiado intensivo en balance para
   el tamaño del Fondo IV.
5. Eficiencia de recursos — descartado por no tener ningún precedente en el
   portafolio de Linzor.

## Fuentes de datos, en el orden en que las usé

1. **SIIS** (siis.ia.supersociedades.gov.co) — ventas, EBITDA/EBIT, balance, flujo
   de caja de cada candidato.
2. **LaNota.com** — rankings sectoriales pagados con cifras ya tabuladas (TI, IPS),
   más rápido que buscar candidato por candidato.
3. **RUES / Cámara de Comercio** — NIT, representante legal, composición
   accionaria. Cobertura parcial: el certificado estándar de una S.A.S. rara vez
   revela el porcentaje accionario detallado.
4. **REPS** (prestadores.minsalud.gov.co) — para dimensionar candidatos de salud por
   número de sedes/servicios cuando no había dato financiero.
5. **Verificación de "¿ya tiene dueño institucional?"** — el paso de mayor
   rendimiento por tiempo invertido: una búsqueda de "[empresa] adquisición" o
   "[empresa] fondo" descarta rápido a cualquier candidato que un fondo global ya se
   haya llevado, antes de gastar tiempo en verificación financiera detallada.
6. **Reseñas de empleados (Indeed/Glassdoor)** — un chequeo rápido y gratuito de
   salud organizacional que resultó más certero que la prensa financiera para
   detectar deterioro operativo: así descarté Asesoftware, cuya caída de ventas de
   45% en el propio SIIS coincidía exactamente con reseñas de empleados que describían
   atrasos de nómina y fuga de talento.

## El archivo de trabajo

[`screening-colombia.xlsx`](./screening-colombia.xlsx) — 33 empresas colombianas,
con una matriz de scoring ponderado sobre 5 criterios: Encaje con Linzor (30%),
Tamaño (15%), Palanca de valor (20%), Ángulo de transacción (20%), Disponibilidad de
datos (15%).

## Empresas descartadas por ya tener sponsor institucional o haber sido adquiridas

| Empresa | Motivo del descarte |
|---|---|
| Siesa | Advent International compró participación mayoritaria en dic. 2024 |
| Digital Ware | H.I.G. Capital, accionista desde feb. 2019 |
| IMAT Oncomédica | Grupo Auna (Enfoca) adquirió el 70% en 2025 |
| Alegra | Riverwood Capital, Serie A de US$22M en jun. 2023 (growth equity) |
| Sonría | Posible ronda de growth equity ya recibida (Dealroom, monto no revelado) |

## Empresas descartadas por no alcanzar el piso de ventas

Xenco (US$4.7M), Novasoft (US$7.7M) y Asesoftware (US$9.9M, con una crisis
financiera confirmada de forma independiente por reseñas de empleados).

## Lo que llegó a la etapa final

Dos candidatos sobrevivieron el embudo con datos financieros limpios y sin sponsor
de PE/VC visible: **Satrack** (el target elegido) y **Sincosoft/Sinco ERP** (el
respaldo). El razonamiento completo de esa decisión final está en
[`04-memo/`](../04-memo/).
