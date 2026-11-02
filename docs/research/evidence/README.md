# Inventario de evidencias — EX01

Mostras da Xunta recollidas o 28/10/2026 e traspaso documental incorporado o 29/10/2026. Non son respostas novas obtidas ao preparar a documentación.

| Ficheiro | Procedencia e tratamento |
| --- | --- |
| `xunta_listaxe_2026-10-28_orixinal.md` | Copia sen modificacións do ficheiro achegado `Markdown pegado(2).md`; contén a resposta entre delimitadores Markdown. |
| `xunta_eventos_2026-10-29_2026-11-11.json` | Extracción do bloque JSON da copia orixinal, sen cambios nos valores. `dataPeticion`: `2026-10-28 20:07:29`. |
| `xunta_evento_157064_2026-10-28.json` | Transcrición da resposta completa compartida polo usuario na conversa, repartida en dúas mensaxes consecutivas. Conserva os campos e valores; cambia a presentación dos espazos. Non é unha descarga HTTP nin unha reconstrución a partir dun resumo. `dataPeticion`: `2026-10-28 20:30:04`. |

## Traspaso da comparación de fontes — 29/10/2026

`EX01_source_comparison_traspaso_2026-10-29.txt` é unha copia sen modificacións de `Texto pegado.txt`, achegado polo usuario. Conserva o relato da revisión manual, os criterios e os resultados provisionais. Non é texto descargado das webs nin unha colección de capturas. A data do nome identifica a incorporación documental; non establece o instante de inspección de cada páxina.

Non se achegaron nesta sesión as capturas da conversa principal. Quedan pendentes de inventario as URL individuais, os rexistros orixinais que sustentan as discrepancias e a programación detallada do Samaín. A URL individual de El aprendiz de arquero no Marcos Valcárcel figura no traspaso; non se volveu verificar nesta entrega. Véxanse os límites e tarefas no [caderno de comparación](../EX01_source_comparison.md).

## Evidencias pendentes da primeira entrega

- JSON completo do detalle `156460`: o contexto accesible comeza a metade da resposta; non se fabrica un ficheiro completo.
- Respostas orixinais de identificación territorial, incluída a consulta con `superior_ine=32` e as coordenadas municipais.
- Captura ou outro rexistro da comprobación do mapa do Teatro Principal.
- Copia do manual oficial, se procede conservala. A documentación inclúe a ligazón e a versión consultada.
- Rexistro das peticións HTTP (URL efectiva, cabeceiras, estado e instante de captura) para futuras recollidas. As mostras actuais non o conteñen.

Non se substitúen estas evidencias históricas por respostas actuais sen identificar a nova data de recollida. Os hashes SHA-256 de `SHA256SUMS` permiten detectar cambios nos ficheiros de evidencia conservados, incluído o traspaso textual.

## Actualización da clasificación — 29/10/2026

[EX01_classification_decisions_2026-10-29.md](EX01_classification_decisions_2026-10-29.md) rexistra as decisións comunicadas directamente polo usuario: 12 inclusións da Xunta, criterio ampliado, comparación de 17 eventos únicos observados e pausa do experimento. É un rexistro documental de decisións, non unha nova evidencia HTTP nin unha transcrición de fichas. O traspaso anterior consérvase como estado histórico, aínda que nel a clasificación figurase pendente.

## Clasificación e validación do centro — 01/11/2026

[EX01_marcos_valcarcel_decisions_2026-11-01.md](EX01_marcos_valcarcel_decisions_2026-11-01.md) rexistra as decisións recibidas (8 inclusións e 1 exclusión), o criterio de acceso e a continuación recibida sobre La Región / Press Club. Non substitúe o programa de invitación da UNED, non achegado aquí. O [contraste documental](../EX01_marcos_valcarcel_overlap.md) identifica os inventarios utilizados, casos próximos e limitacións para o resultado de 25 eventos observados. Non se descargaron novas fichas nin se resolveron as incidencias de La Región / Press Club. A continuación incorpora a diferenza interna listaxe/ficha de Pateiro e a coincidencia horaria das ERUs, segundo a comunicación do usuario.

## Investigación de La Región / Press Club — 02/11/2026

[EX01_laregion_traspaso_2026-11-02.txt](EX01_laregion_traspaso_2026-11-02.txt) conserva sen modificacións o ficheiro achegado `Texto pegado(1).txt`. É un traspaso de investigación e decisións, non unha captura das fontes. A data identifica a incorporación documental, non o instante de inspección de cada páxina. O [caderno de comparación](../EX01_source_comparison.md) incorpora o inventario de sete actividades, o contraste cos 25 anteriores, duplicados, exclusións e observacións de calidade. Non se achegaron as URL individuais, capturas ou programas completos; quedan explicitamente pendentes. As versións horarias e de datas non se resolven por inferencia.

## Ampliación comunicada de 32 a 89 — 02/11/2026

A [auditoría da ampliación](../EX01_expansion_audit.md) identifica a instrución directa do usuario (U), a recuperación de resumos de conversación (H0–H3) e consultas limitadas de páxinas (V1–V3). Non se recibiu un ficheiro co inventario completo dos 57 adicionais. As 23 actuacións recupéranse de resumos anteriores do asistente, non de publicacións primarias arquivadas; non demostran celebración efectiva. O documento conserva os rexistros parciais e o saldo sen inventario, sen fabricar fichas. As URL, datos observados e fallos de acceso están rexistrados, pero non se gardaron respostas HTTP completas nin capturas.

### Integridade dos traspasos anteriores

Na revisión detectáronse dous hashes que non coincidían cos bytes xa integrados en `main`: os traspasos `EX01_source_comparison_traspaso_2026-10-29.txt` e `EX01_laregion_traspaso_2026-11-02.txt`. Contrastáronse coas copias achegadas: o texto coincide tras normalizar CRLF/LF; os finais de liña cambiaron na integración anterior. Non se editan os ficheiros de evidencia. Actualízanse só os hashes para os bytes realmente conservados. As afirmacións de copia sen modificacións dos apartados anteriores describen a preparación orixinal, non identidade binaria tras esa normalización.
