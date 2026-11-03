# EX01 — Radio Liverdade: acceso estruturado e reutilización

Data: 03/11/2026 · Estado: fonte candidata, valoración provisional.

## Alcance e procedencia

Avaliación técnica e das condicións publicadas, mantendo o municipio de Ourense e a xanela **29/10/2026–11/11/2026, ambos incluídos**. **Non se modifica o inventario de 89 eventos únicos provisionais reconciliados nominalmente**, nin se incorporan actividades vistas nas exportacións. Non se implementou un recolector, non se iniciou o MVP e non se engadiron dependencias.

Diferéncianse catro clases de evidencia:

- **Comprobado nesta sesión:** inspección local de dez ICS recollidos anteriormente; consulta do aviso legal e da listaxe pública; convención `DTEND` contrastada co RFC.
- **Seguimento manual comunicado polo usuario:** descarga directa da quinta páxina, mostra HTML–ICS de 12/12, observación de Creative Commons, intento de `robots.txt` e preparación do correo.
- **Inferencia técnica:** viabilidade dunha futura consulta automatizada e utilidade de `UID` como chave dentro da fonte; non se probaron como sistema completo.
- **Pendente:** integridade global, condicións de uso aplicables á consulta periódica e permisos de almacenamento/republicación.

Fontes:

- Web: <https://radioliverdade.com/>
- Axenda: <https://radioliverdade.com/axenda/>
- Listaxe: <https://radioliverdade.com/axenda/listaxe/>
- Aviso legal: <https://radioliverdade.com/aviso-legal/>

Radio Liverdade actúa como medio e axenda agregadora; publicar un evento non a converte automaticamente na súa organizadora. A cobertura municipal e supramunicipal require filtrado. O seguimento identifica WordPress e The Events Calendar. Nos ICS inspeccionados, `PRODID` inclúe `Radio Liverdade - ECPv6.17.4.1`; é un indicio concordante do produtor, non unha auditoría da instalación ou da súa configuración.

## Acceso e integridade: resultados e límites

URL probada no seguimento manual:

```text
https://radioliverdade.com/axenda/listaxe/page/5/?tribe-bar-date=2026-10-29&ical=1
```

O usuario informa de descarga correcta por URL directa, sen interacción cos botóns, e de exportacións de distintas páxinas. **Nesta sesión non se puido repetir a descarga desa URL nin acceder á súa páxina HTML correspondente coa ferramenta de consulta.** Non se interpreta esa limitación como inexistencia do mecanismo; a evidencia local conserva exportacións reais, pero non un rexistro HTTP que as vincule individualmente con cada URL e modalidade.

| Proba | Resultado | Estado da evidencia |
| --- | --- | --- |
| Estrutura de dez ficheiros | 30 bloques `VEVENT` en cada un | Recalculado directamente sobre os bytes dispoñibles |
| UID dentro de cada ficheiro | 30 distintos en cada exportación | Comprobado nesta mostra, non garantía de estabilidade futura |
| Estándar / Outlook | Mesmo contido dos eventos; diferenza `X-WR-CALNAME:Radio Liverdade` | Par identificado abaixo; os papeis estándar/Outlook proceden do seguimento |
| Solapamento | Hai UIDs compartidos entre exportacións | Comprobado; páxinas non equivalen a lotes disxuntos |
| Quinta páxina HTML fronte a ICS | 12 visibles; os 12 no ICS de 30; intervalo máis amplo | Comprobación manual previa relatada, non reproducida nesta sesión |

A mostra 12/12 non detectou omisións, pero **non demostra a integridade global** nin a equivalencia entre a paxinación HTML e a exportación. Falta conservar esa listaxe HTML e a correspondencia exacta URL–ficheiro para reproducir a proba.

### Inspección dos ficheiros dispoñibles

Véxase o [informe de inspección](evidence/radio_liverdade_ics_inspection_2026-11-03.json), con nomes, procedencia, hashes, tamaños e presenza de campos. Os ICS completos non se incorporan ao repositorio; consérvanse aquí os resultados técnicos da inspección, sen descricións nin imaxes dos eventos.

- Dez ficheiros, nove hashes distintos: `radio-liverdade-2a6c4fd473d.ics` e a copia con sufixo `(1)` son idénticos en bytes. Non se consideran dúas mostras independentes.
- 300 rexistros ao sumar os dez ficheiros e unión de 120 UIDs. **Estas cifras describen a mostra técnica, non eventos culturais novos nin un cambio dos 89.** Inclúen duplicacións e datas alleas á xanela.
- O par `radio-liverdade-0ae85c4d811.ics` / `radio-liverdade-30d3631d02c.ics` ten os mesmos bloques de eventos. Eliminando no primeiro a liña `X-WR-CALNAME:Radio Liverdade`, o resto dos bytes coincide co segundo.
- Os pares `20dbfb5ef02` / `b5b81dd8217` e `0ea3a290a1f` / `20dbfb5ef02` comparten 18 UIDs por par. Non se asigna un número de páxina aos ficheiros a partir do seu nome.

## Estrutura e interpretación

| Campo / propiedade observada | Uso posible e límite |
| --- | --- |
| `UID` | Identidade dentro da fonte; útil para deduplicar exportacións solapadas. Se hai recorrencias, considerar tamén a identidade da instancia. Non resolve identidade entre fontes distintas. |
| `DTSTART`, `DTEND` | Datas e horas. Zona identificada: `Europe/Madrid`; conservar o tipo DATE ou DATE-TIME e o fuso. |
| `DTSTAMP`, `CREATED`, `LAST-MODIFIED` | Metadatos temporais presentes. Non se probou longitudinalmente que `LAST-MODIFIED` detecte todos os cambios, cancelacións ou retiradas. |
| `SUMMARY`, `DESCRIPTION` | Título e descrición; a presenza da propiedade non garante contido útil. |
| `URL`, `LOCATION` | Ligazón á publicación e lugar; poden requirir normalización e contraste. Non confundir lugar con organizador. |
| `CATEGORIES`, `ATTACH` | Categorías e referencia a recurso, sen garantía de completitude nin permiso de uso da imaxe. `CATEGORIES` non aparece en todos os rexistros da mostra. |
| `REFRESH-INTERVAL;VALUE=DURATION:PT1H`, `X-PUBLISHED-TTL:PT1H` | Indicación de actualización recomendada do calendario; **non proba de que cada evento se actualice cada hora**. |

Segundo [RFC 5545, sección 3.6.1](https://datatracker.ietf.org/doc/html/rfc5545#section-3.6.1), `DTEND` é un límite non inclusivo. Nun evento de día completo, a data final non se debe presentar como outro día de actividade. É unha convención do formato, non unha garantía de que cada rexistro da fonte estea ben introducido.

## Calidade e incidencias da mostra

- Cobertura xeográfica mixta segundo o seguimento manual: cómpre distinguir municipio, sede e posibles localizacións incompletas antes de incluír actividades.
- A análise local identifica entre 13 e 23 descricións baleiras por ficheiro de 30. Son cifras por exportación solapada, non unha porcentaxe de eventos únicos sen descrición.
- Aparece `Latno` en `LOCATION` de tres exportacións; non son necesariamente tres eventos distintos. Conservar valor orixinal e corrección proposta sen substitución silenciosa.
- A repetición de UIDs confirma solapamentos; non se validou a súa estabilidade a longo prazo. A deduplicación entre fontes require título/identidade, datas, sede e pertenza a eventos compostos, non só UID.
- Non se ensaiaron todas as páxinas, períodos, recorrencias, cambios de estado ou modificacións sucesivas. Campo estruturado non equivale a dato completo, correcto ou fiable.

Non se resolven nesta entrega as discrepancias de eventos xa rexistradas no caderno xeral, incluídas as versións de Radio Liverdade. A inspección técnica non autoriza altas, baixas nin cambios de identidade no inventario.

## Condicións publicadas e contacto

O [aviso legal](https://radioliverdade.com/aviso-legal/), sección «Propiedade intelectual e industrial», consultado o 03/11/2026, establece restricións sobre reprodución, almacenamento permanente, difusión e usos públicos ou comerciais, condicionados ao consentimento previo expreso por escrito. Consérvase esta observación documental sen concluír autorización para datos básicos, descricións ou imaxes.

O usuario observou unha referencia visual a CC BY-NC noutra páxina. Non se identificou aquí o seu ámbito nin a súa relación co aviso legal. A consulta anterior de `robots.txt` non puido completarse; nesta actualización non se determina ningunha directriz de rastrexo. Nin o calendario público nin unha directriz de rastrexo substitúen a aclaración das condicións de reutilización.

Preparouse na investigación un borrador para `info@radioliverdade.com`, sobre consulta periódica por ICS, almacenamento e presentación de datos básicos con atribución/enlace e condicións de descricións/imaxes. **Non consta envío, resposta nin autorización concedida.** Nesta sesión non se enviou ningún correo e non se reconstrúe o borrador ausente.

## Valoración provisional e pendentes

| Dimensión | Valoración |
| --- | --- |
| Accesibilidade técnica | Favorable segundo exportacións inspeccionadas e descarga directa relatada |
| Calidade | Útil, con baleiros e normalización pendente |
| Xeografía | Mixta; require filtrado municipal |
| Integridade global | Non demostrada; só mostra puntual 12/12 relatada |
| Consulta periódica automatizada | Tecnicamente plausible; condicións de uso por aclarar; recolector completo non probado |
| Almacenamento e republicación | Pendentes de autorización ou aclaración |
| Descricións e imaxes | Non asumir permisos |

Próximos pasos documentais: conservar a proba HTML–ICS e a trazabilidade por URL/modalidade, aclarar o ámbito da referencia CC BY-NC, completar a revisión de `robots.txt` e obter resposta ás preguntas de uso. As probas futuras de integridade e estabilidade deberán distinguir cambios reais de datos de cambios de exportación. Non se executan nesta entrega nin se implementa un recolector.

**Conclusión:** fonte candidata tecnicamente prometedora, con calidade e integridade aínda limitadas pola mostra e reutilización sen aclarar. O EX01 segue aberto e o reconto continúa en **89 eventos únicos provisionais**.
