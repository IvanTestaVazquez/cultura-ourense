# Experimento 01 — API da Axenda de Cultura da Xunta

Estado: clasificación completada; EX01 en pausa · Mostra: 28/10/2026 · Actualización: 29/10/2026.

## Contexto e obxectivo

Cultura Ourense é un proxecto de portfolio en fase de Product Discovery, orientado ao descubrimento de eventos culturais no municipio de Ourense. O Experimento 01 estuda a cobertura e o solapamento de fontes. Este caderno documenta a primeira análise da API da Xunta; non define o MVP nin a arquitectura.

## Criterios de evidencia

- **Documentado:** consta no manual oficial, con sección de referencia.
- **Verificado na evidencia conservada:** comprobable nos ficheiros desta carpeta.
- **Comprobación previa relatada:** resultado rexistrado na conversa de investigación, sen toda a evidencia orixinal conservada aquí.
- **Hipótese:** explicación pendente de contraste; non é unha conclusión.

As datas `dataPeticion` transcríbense como as devolveu a fonte, sen atribuírlles un fuso horario non indicado no JSON. Non se repetiron as peticións da API nesta entrega.

## Fonte e documentación oficial

- API base: <https://www.cultura.gal/v1/axenda>
- Manual: <https://ficheiros-web.xunta.gal/cultura/servizo-web/Manual_Servizo%20Web_Axenda_Cultura.pdf>

Consultouse o manual oficial, versión 1.9 (27 páxinas). A sección 1 documenta REST, a URL base e os formatos JSON/XML seleccionables mediante `Accept` ou extensión. As seccións 3.5, 4.1 e 4.2 tratan os recursos territoriais, a listaxe e o detalle de eventos. Esta referencia documental non demostra por si soa o comportamento actual do servizo. O PDF non se incorpora nesta entrega.

## Identificación territorial

| Dato | Valor | Procedencia |
| --- | --- | --- |
| Concello | Ourense | JSON da listaxe e comprobación previa |
| `tid` do concello | `403` | JSON da listaxe |
| Código INE do concello | `320548` | JSON da listaxe |
| Código INE da provincia | `32` | Comprobación previa relatada |
| Identificador interno da provincia | `34` | Comprobación previa relatada |
| Concellos devoltos con `superior_ine=32` | `92` | Comprobación previa relatada |

Falta conservar a resposta territorial orixinal. Non se debe confundir o identificador interno co código INE.

## Consulta de eventos

Petición rexistrada na investigación:

```text
https://www.cultura.gal/v1/axenda/eventos.json?idioma=gl&concello=403&inicio=2026-10-29&fin=2026-11-11&limite=20&paxina=0
```

Período solicitado: 29/10/2026–11/11/2026. Comprobación: 28/10/2026.

A evidencia achegada contén `dataPeticion: 2026-10-28 20:07:29`, `totalResultados: 12`, `elementosPorPaxina: 20` e 12 elementos en `listaAxenda`, todos asociados ao concello `403`. A URL da petición procede da conversa: o JSON non inclúe un rexistro HTTP que a vincule por si só á resposta.

Os 12 rexistros recuperados clasificáronse como culturais e incluídos cos [criterios metodolóxicos do experimento](EX01_source_comparison.md#criterios-metodolóxicos-provisionais). Resultado: **12 incluídos, 0 excluídos**. É o reconto desta mostra, non unha medida da oferta cultural total.

### Mostra conservada

Títulos e datas procedentes do JSON; elimínanse unicamente os espazos finais dos títulos para a presentación.

| ID | Título | Inicio | Fin | Espazo asociado |
| --- | --- | --- | --- | --- |
| 157064 | Redescubrindo Ourense : A Esmorga - xoves 29 outubro | 2026-10-29 16:30:00 | 2026-10-29 16:30:00 | Biblioteca Pública de Ourense |
| 157066 | Redescubrindo Ourense. A memoria en femenino da cidade. | 2026-10-30 11:30:00 | 2026-10-30 11:30:00 | Biblioteca Pública de Ourense |
| 156460 | A serie clopen | 2026-10-30 20:00:00 | 2026-10-30 20:00:00 | Teatro Principal |
| 157005 | Entre as cubertas dos libros | 2026-10-31 12:00:00 | 2026-10-31 12:00:00 | Biblioteca Pública de Ourense |
| 157020 | Máis libros = Máis libres | 2026-10-05 12:00:00 | 2026-10-31 14:00:00 | Biblioteca Pública de Ourense |
| 157007 | Mes dos libros prohibidos: que é a censura? | 2026-10-05 11:00:00 | 2026-10-31 14:00:00 | Biblioteca Pública de Ourense |
| 157095 | Peza do mes: Fotografía do arco neomudéxar en homenaxe ao Padre Feijoo | 2026-10-01 10:00:00 | 2026-10-31 20:00:00 | Museo Arqueolóxico Provincial de Ourense |
| 157018 | Mostra de teares tradicionais | 2026-10-08 09:00:00 | 2026-10-31 21:00:00 | Biblioteca Pública de Ourense |
| 157319 | Contiños na biblio - Contacontos pequenos científicos - martes 3 | 2026-11-03 18:00:00 | 2026-11-03 18:00:00 | Biblioteca Pública de Ourense |
| 157321 | Xogando coas letras - mércores 4 | 2026-11-04 18:00:00 | 2026-11-04 18:00:00 | Biblioteca Pública de Ourense |
| 157333 | Poden ser sexistas as campañas institucionais contra o sexismo? | 2026-11-05 18:00:00 | 2026-11-05 18:00:00 | Biblioteca Pública de Ourense |
| 157323 | Obradoiro de xogos de mesa con Alba Polo | 2026-11-07 12:00:00 | 2026-11-07 12:00:00 | Biblioteca Pública de Ourense |

Hai actividades que comezan antes do 29/10 e rematan dentro do período consultado. A mostra é compatible cun filtro por solapamento temporal; non permite concluír a regra completa, a inclusividade dos límites nin o tratamento de todos os casos. Non se interpreta `dataFin` igual a `dataInicio` como unha duración real de cero minutos.

## Clasificación cultural — 29/10/2026

A clasificación foi comunicada polo usuario tras a revisión na conversa principal; véxase o [rexistro de decisións](evidence/EX01_classification_decisions_2026-10-29.md). As xustificacións seguintes vinculan cada inclusión cos criterios operativos, sen atribuír novos campos á API nin afirmar unha nova verificación das fichas nesta sesión.

| ID | Evento | Decisión | Encaixe no criterio |
| --- | --- | --- | --- |
| 157064 | Redescubrindo Ourense : A Esmorga - xoves 29 outubro | Incluído | Roteiro literario e divulgación humanística |
| 157066 | Redescubrindo Ourense. A memoria en femenino da cidade. | Incluído | Divulgación histórica e social mediante roteiro |
| 156460 | A serie clopen | Incluído | Artes escénicas |
| 157005 | Entre as cubertas dos libros | Incluído | Dinamización cultural infantil e fomento da lectura; inclusión confirmada expresamente |
| 157020 | Máis libros = Máis libres | Incluído | Fomento da lectura mediante mostra bibliográfica; inclusión confirmada expresamente |
| 157007 | Mes dos libros prohibidos: que é a censura? | Incluído | Literatura e divulgación sobre a censura |
| 157095 | Peza do mes: Fotografía do arco neomudéxar en homenaxe ao Padre Feijoo | Incluído | Divulgación do patrimonio histórico |
| 157018 | Mostra de teares tradicionais | Incluído | Exposición de patrimonio cultural |
| 157319 | Contiños na biblio - Contacontos pequenos científicos - martes 3 | Incluído | Narración oral e divulgación científica infantil |
| 157321 | Xogando coas letras - mércores 4 | Incluído | Fomento da lectura e comprensión lectora |
| 157333 | Poden ser sexistas as campañas institucionais contra o sexismo? | Incluído | Divulgación social mediante conferencia sobre campañas contra o sexismo; inclusión confirmada expresamente |
| 157323 | Obradoiro de xogos de mesa con Alba Polo | Incluído | Dinamización cultural mediante obradoiro de xogos de mesa; inclusión confirmada expresamente |

Todos os rexistros da mostra quedan incluídos; non hai exclusións nin casos pendentes dentro destes 12. A confirmación dos catro casos sinalados non implica incluír automaticamente calquera actividade de temática social ou calquera xogo: o criterio segue a requirir avaliar cada caso. As categorías da API son datos da fonte, non a decisión cultural do experimento.

## Endpoint de detalle

Consultas utilizadas na investigación previa:

- <https://www.cultura.gal/v1/axenda/eventos/156460.json?idioma=gl>
- <https://www.cultura.gal/v1/axenda/eventos/157064.json?idioma=gl>

| Campo | 156460 — A serie clopen | 157064 — Redescubrindo Ourense: A Esmorga |
| --- | --- | --- |
| Espazo asociado | Teatro Principal | Biblioteca Pública de Ourense |
| `espazoId` | `null` | `1023` (número no evento; cadea no lugar) |
| Lonxitude | `-7.86389619112` | `-7.8593069` |
| Latitude | `42.335549382851` | `42.338061` |
| Data e hora da actividade | 30/10/2026 20:00 | 29/10/2026 16:30 |

A listaxe conservada permite comprobar os espazos, as coordenadas e as datas. A comparación cos detalles foi realizada na sesión previa. Os detalles achegan descrición HTML, público, tipo de entrada, entidade relacionada, data de actualización e celebracións; un campo pode estar baleiro.

### EX01-XUNTA-001 — Localización do Teatro Principal

**Incidencia confirmada na investigación previa.** As coordenadas do evento coinciden exactamente coas municipais segundo a comparación relatada. Na web observouse o marcador na Praza Maior, en lugar do Teatro Principal. O detalle conserva as coordenadas e non resolve a incidencia.

A listaxe conserva o valor observado, pero faltan a resposta territorial, o detalle completo e unha captura do mapa para facer reproducible toda a comprobación. Esta entrega non volveu inspeccionar o mapa.

### EX01-XUNTA-002 — Punto de encontro dun roteiro

**Observación verificada no detalle achegado na conversa.** A descrición de A Esmorga indica como inicio a Consellería de Sanidade, na avenida de Zamora, mentres o espazo asociado é a Biblioteca Pública de Ourense.

A diferenza é coherente coa natureza itinerante do roteiro e non se clasifica como erro. Neste exemplo o punto de encontro está en texto libre; non se pode asumir que as coordenadas do espazo asociado indiquen onde debe presentarse unha persoa. A observación non se xeneraliza a todos os eventos.

### EX01-H01 — `espazoId` e coordenadas municipais

**Hipótese aberta:** a ausencia de `espazoId` podería estar relacionada co uso das coordenadas municipais como valor substitutivo. Os dous exemplos analizados son compatibles con esta explicación, pero non demostran causalidade nin unha regra xeral. Cómpre ampliar a mostra e buscar contraexemplos antes de aceptala.

## Evidencias e trazabilidade

Véxase [o inventario de evidencias](evidence/README.md). Consérvase o ficheiro achegado sen modificacións e unha extracción do seu bloque JSON, validada por equivalencia de datos. Non se reconstrúen respostas ausentes a partir de resumos.

## Conclusións provisionais e pendentes

A resposta conservada e as comprobacións previas amosan información estruturada útil. Non se conclúe que a API sexa suficiente como fonte única. Queda por avaliar:

- Cobertura e solapamento coa axenda do Concello de Ourense e outras fontes, mantendo o mesmo período; véxase a [comparación de fontes](EX01_source_comparison.md).
- Precisión xeográfica e interpretación do espazo asociado fronte ao punto de encontro.
- Semántica dos intervalos de datas e límites da consulta.
- Completitude, actualización, cancelacións, aprazamentos e posibles duplicados.
- Condicións de reutilización dos datos; a dispoñibilidade pública non establece unha licenza.

Actualización do 29/10/2026: a fonte municipal identificada é a [axenda do Concello](https://ourense.gal/es/proximoseventos/), en substitución da referencia anterior a Turismo Ourense. A exploración manual e os seus límites recóllense no [caderno de comparación](EX01_source_comparison.md). A clasificación queda completada: 12 incluídos e 0 excluídos. A comparación comunicada co Concello ofrece **17 eventos únicos observados** (12 + 5, sen duplicados identificados). O EX01 queda en pausa; a posible ampliación a Marcos Valcárcel e La Región é traballo futuro. Non se garante exhaustividade nin se estima a cobertura total de Ourense.
