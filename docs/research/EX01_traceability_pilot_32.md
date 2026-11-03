# EX01 — Matriz documental de trazabilidade dos 89 eventos provisionais

Estado: ampliación documental para revisión · Data: 03/11/2026 · Referencia consolidada consultada: `origin/main` en `d5ffc559213223df2e6cdb6401ca2005fdba0ff8`.

## Alcance e criterios de lectura

Ampliación do piloto validado: consérvanse as 32 filas iniciais, AT-01–47, TM-01–14 e os oito source_id anteriores. Engádense exclusivamente as 57 unidades xa reconciliadas en E8: MUS 23 + AMP 29 + PV 4 + FOR 1. O nome do ficheiro conserva a orixe piloto para reutilizar o documento. Non se alteran os inventarios consolidados, as evidencias orixinais nin os 89 eventos únicos provisionais; non se realizan consultas externas.

A matriz é completa na representación nominal dos 89 eventos, pero incompleta nas atribucións a fontes. Unha fila de inventario non garante unha fonte publicadora identificada. As lagoas non se completan coa sede ou coa procedencia U/H/C.

O grupo de incorporación é Xunta/MUN/MV/LR/MUS/AMP/PV/FOR; o `source_id` identifica unha canle publicadora, non unha sede, organizador ou código U/H/C. Os identificadores numéricos da Xunta e os MUN/MV/LR existentes non se cambian. MUN-04, MUN-05 e MV-04 seguen excluídos do piloto segundo os inventarios.

`—` significa dato descoñecido, non precisado ou non aplicable segundo a nota: non crea unha afirmación negativa. Nos casos con conflitos temporais de data do piloto, os campos temporais do inventario deixan de mesturar alternativas e remiten á táboa B.2; os valores anteriores quedan alí conservados, non eliminados nin reinterpretados. Nos casos sen conflito non se introduce outra estrutura temporal. Un final non documentado non se completa por inferencia.

## Referencias documentais

| Código | Documento e localizador |
| --- | --- |
| E1 | [JSON da listaxe da Xunta](evidence/xunta_eventos_2026-10-29_2026-11-11.json), array `listaAxenda`, campo `id`. Inclúe as URL individuais. |
| E2 | [Caderno da Xunta](EX01_xunta_api.md), §Mostra conservada, §Clasificación cultural e incidencias EX01-XUNTA-001/002. |
| E3 | [Detalle157064 conservado](evidence/xunta_evento_157064_2026-10-28.json), `evento`, corpo e lugar asociado. |
| E4 | [Comparación de fontes](EX01_source_comparison.md), sección e fila/incidencia indicada en cada rexistro. As URL xerais das fontes constan nos seus apartados. |
| E5 | [Traspaso inicial](evidence/EX01_source_comparison_traspaso_2026-10-29.txt), §§5–7: Concello, centro e La Región. |
| E6 | [Contraste do centro](EX01_marcos_valcarcel_overlap.md), §Contraste por evento e §Resultado e alcance. |
| E7 | [Traspaso La Región](evidence/EX01_laregion_traspaso_2026-11-02.txt), §§2–7: incorporacións, coincidencias e calidade. |
| E8 | [Auditoría ampliada](EX01_expansion_audit.md), §Fontes e comprobacións limitadas, V1. Inclúe agora as táboas MUS/AMP/PV/FOR, agrupacións e V1/V2/V3; conserva a referencia anterior a MV-03. |
| E9 | [Radio Liverdade](EX01_radio_liverdade.md), §Inspección dos ficheiros dispoñibles: estatísticas técnicas sen mapeamento dos 89. Non proba novas atribucións individuais nesta matriz. |
| E10 | [Complemento da reconciliación](evidence/EX01_expansion_complement_2026-11-02.txt), §§2–8; comprobacións e carteis relatados, non orixinais arquivados. |

## Catálogo de fontes identificadas

Os IDs seguintes son estables para este documento de investigación. Os nomes reproducen a atribución anterior; non pretenden identificar persoas xurídicas non documentadas. La Región e Press Club non se fusionan e non se atribúe ao segundo unha titularidade por dedución. Os locais que só figuran como sedes non xeran entradas no catálogo.

| source_id | source_name | entity | channel | notes |
| --- | --- | --- | --- | --- |
| SRC-XUNTA | Xunta — Axenda de Cultura | Xunta de Galicia | Axenda de Cultura / API | Fonte E1/E2. Non equivale aos organizadores ou espazos dos seus eventos. |
| SRC-CONCELLO | Concello — axenda municipal | Concello de Ourense | Axenda municipal | E4 §Concello de Ourense; nome do publicador, non atribución automática de todos os espazos municipais. |
| SRC-MV | Centro Cultural Marcos Valcárcel — axenda | Centro Cultural Marcos Valcárcel; responsable xurídico/editorial non precisado | Axenda / programación do centro | E4 §Centro Cultural Marcos Valcárcel. A identidade da canle publicadora está documentada; non se deduce da sede de cada evento. |
| SRC-LAREGION | La Región — axenda/artigos | La Región; sociedade titular non precisada | Axenda e artigos; superficie concreta só cando consta | E4 §La Región e Press Club. Mantense separada de SRC-PRESSCLUB; non asumir independencia de todas as súas canles. |
| SRC-PRESSCLUB | Press Club — Foro/promocións | — (entidade responsable non identificada nesta matriz) | Press Club / Foro e promocións de entradas | E4/E7 documentan a vinculación con La Región; non se inventa identidade xurídica nin se fusionan as fontes. |
| SRC-TURISMO | Turismo de Ourense — axenda | — (responsable editorial concreto non precisado) | Axenda turística municipal | E4 §EX01-COMP-005/006/010; non é a mesma canle documental que a axenda SRC-CONCELLO. |
| SRC-RADIOLIVERDADE | Radio Liverdade — axenda | Radio Liverdade | Axenda agregadora | E8 V1 e E9. Non organizadora por defecto; as atribucións individuais proceden de E8 V1, non das estatísticas agregadas ICS de E9. |
| SRC-LICEO | Liceo de Ourense — axenda | Liceo de Ourense | Axenda do Liceo | E4 EX01-COMP-005. Aquí consta unha publicación, ademais de coincidir coa sede; iso non se xeneraliza a todos os eventos do Liceo. |
| SRC-CINECLUBE | Cineclube Padre Feijoo — blog de programación | Cineclube Padre Feijoo | Blog / programación | E8: portada accesible, fichas específicas bloqueadas. A atribución dos tres filmes é probable, non confirmación da publicación individual. |
| SRC-TEATRO | Teatro Principal — programación | Teatro Principal; responsable editorial non precisado | Programación | E4 EX01-COMP-012/013 nomea expresamente a canle; non se atribúe por ser sede. |
| SRC-MAPOU | Museo Arqueolóxico Provincial de Ourense — programación | Museo Arqueolóxico Provincial de Ourense | Programación | E10 §4 identifica a fonte primaria utilizada para AMP-11–13. |
| SRC-UVIGO | Universidade de Vigo — axenda institucional | Universidade de Vigo | Axenda / información institucional | E10 §5 atribúe expresamente AMP-15; canle diferenciada da Facultade. |
| SRC-FRRII | Facultade de Relacións Internacionais — eventos | Facultade de Relacións Internacionais, Universidade de Vigo | Web da facultade / eventos | E10 §5 achega URL específica; ser organizadora non é o único apoio da atribución. |
| SRC-PONTEVELLA | Ponte Vella — carteis de programación | Ponte Vella; responsable editorial non precisado | Carteis do 25.º aniversario | E10 §2 atribúe expresamente os carteis PV-01–04. Non se estende a AMP-27 por compartir sede. |
| SRC-FORASTEIRO-IG | Cafetería Forasteiro — Instagram | Cafetería Forasteiro | Publicación do establecemento en Instagram | E10 §3 confirma a canle de FOR-03, sen URL. Non se estende a outras actividades pola sede. |
| SRC-CHINITA-IG | Feria de la Chinita Galicia — perfil de Instagram | — (titular do perfil non identificado) | Perfil de Instagram | E10 §5: https://www.instagram.com/feriadelachinitagalicia/ é perfil, non URL específica dun post. |

As dúas publicacións anónimas de CatArte non teñen fila neste catálogo nin `source_id`. A súa etiqueta pendente consérvase en B, coa mesma atribución orixinal. A relación potencial entre canles dunha organización non altera por si soa os recontos.

## A. Inventario dos 89 eventos

Unha fila por unidade xa acordada. `notes` conserva horas sen conflito, agrupacións e localizacións asociadas; unha sede asociada non é necesariamente o punto de encontro. Non se cobren os cinco lugares municipais por suposición. Non se identifican organizadores a partir da sede.

| event_id | title | start_date | end_date | venue | incorporation_group | notes | evidence_reference |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 157064 | Redescubrindo Ourense : A Esmorga - xoves 29 outubro | 2026-10-29 | 2026-10-29 | Biblioteca Pública de Ourense | Xunta | Horas publicadas: 16:30:00 / 16:30:00. Non inferir duración real cando coinciden. EX01-XUNTA-002: inicio do roteiro na Consellería de Sanidade (avda. de Zamora), distinto do espazo asociado; non erro automático. | E1, `listaAxenda`, `id=157064`; E2 §Mostra conservada; E3 §evento |
| 157066 | Redescubrindo Ourense. A memoria en femenino da cidade. | 2026-10-30 | 2026-10-30 | Biblioteca Pública de Ourense | Xunta | Horas publicadas: 11:30:00 / 11:30:00. Non inferir duración real cando coinciden. | E1, `listaAxenda`, `id=157066`; E2 §Mostra conservada |
| 156460 | A serie clopen | 2026-10-30 | 2026-10-30 | Teatro Principal | Xunta | Horas publicadas: 20:00:00 / 20:00:00. Non inferir duración real cando coinciden. EX01-XUNTA-001: coordenadas municipais, non do teatro. | E1, `listaAxenda`, `id=156460`; E2 §Mostra conservada |
| 157005 | Entre as cubertas dos libros | 2026-10-31 | 2026-10-31 | Biblioteca Pública de Ourense | Xunta | Horas publicadas: 12:00:00 / 12:00:00. Non inferir duración real cando coinciden. | E1, `listaAxenda`, `id=157005`; E2 §Mostra conservada |
| 157020 | Máis libros = Máis libres | 2026-10-05 | 2026-10-31 | Biblioteca Pública de Ourense | Xunta | Horas publicadas: 12:00:00 / 14:00:00. Non inferir duración real cando coinciden. | E1, `listaAxenda`, `id=157020`; E2 §Mostra conservada |
| 157007 | Mes dos libros prohibidos: que é a censura? | 2026-10-05 | 2026-10-31 | Biblioteca Pública de Ourense | Xunta | Horas publicadas: 11:00:00 / 14:00:00. Non inferir duración real cando coinciden. | E1, `listaAxenda`, `id=157007`; E2 §Mostra conservada |
| 157095 | Peza do mes: Fotografía do arco neomudéxar en homenaxe ao Padre Feijoo | 2026-10-01 | 2026-10-31 | Museo Arqueolóxico Provincial de Ourense | Xunta | Horas publicadas: 10:00:00 / 20:00:00. Non inferir duración real cando coinciden. | E1, `listaAxenda`, `id=157095`; E2 §Mostra conservada |
| 157018 | Mostra de teares tradicionais | 2026-10-08 | 2026-10-31 | Biblioteca Pública de Ourense | Xunta | Horas publicadas: 09:00:00 / 21:00:00. Non inferir duración real cando coinciden. | E1, `listaAxenda`, `id=157018`; E2 §Mostra conservada |
| 157319 | Contiños na biblio - Contacontos pequenos científicos - martes 3 | 2026-11-03 | 2026-11-03 | Biblioteca Pública de Ourense | Xunta | Horas publicadas: 18:00:00 / 18:00:00. Non inferir duración real cando coinciden. | E1, `listaAxenda`, `id=157319`; E2 §Mostra conservada |
| 157321 | Xogando coas letras - mércores 4 | 2026-11-04 | 2026-11-04 | Biblioteca Pública de Ourense | Xunta | Horas publicadas: 18:00:00 / 18:00:00. Non inferir duración real cando coinciden. | E1, `listaAxenda`, `id=157321`; E2 §Mostra conservada |
| 157333 | Poden ser sexistas as campañas institucionais contra o sexismo? | 2026-11-05 | 2026-11-05 | Biblioteca Pública de Ourense | Xunta | Horas publicadas: 18:00:00 / 18:00:00. Non inferir duración real cando coinciden. | E1, `listaAxenda`, `id=157333`; E2 §Mostra conservada |
| 157323 | Obradoiro de xogos de mesa con Alba Polo | 2026-11-07 | 2026-11-07 | Biblioteca Pública de Ourense | Xunta | Horas publicadas: 12:00:00 / 12:00:00. Non inferir duración real cando coinciden. | E1, `listaAxenda`, `id=157323`; E2 §Mostra conservada |
| MUN-01 | Centenario dos Grandes Voos da Aviación Española (1926–1935) | 2026-10-16 | 2026-10-31 | — (non transcrito por rexistro) | MUN | Exposición: unha unidade; tamén relatada en La Región. | E4 §Concello de Ourense, fila `MUN-01`; E5 §5 |
| MUN-02 | Moi Animal — Xosé A. Touriñán | 2026-10-30 | — | — (non transcrito por rexistro) | MUN | Artes escénicas. | E4 §Concello de Ourense, fila `MUN-02`; E5 §5 |
| MUN-03 | Samaín 2026 en Ourense | 2026-10-31 | — | — (non transcrito por rexistro) | MUN | Evento composto; non separar obradoiros/desfile/concerto; programa completo pendente. | E4 §Concello de Ourense, fila `MUN-03`; E5 §5 |
| MUN-06 | Shado — Cleptómago | 2026-11-06 | — | — (non transcrito por rexistro) | MUN | Artes escénicas. | E4 §Concello de Ourense, fila `MUN-06`; E5 §5 |
| MUN-07 | De Simba a Kiara — Tributo ao Rei León | 2026-11-08 | — | — (non transcrito por rexistro) | MUN | Espectáculo cultural. | E4 §Concello de Ourense, fila `MUN-07`; E5 §5 |
| MV-01 | Juan Lobato: «Ética e política» | — (conflito aberto; ver afirmacións temporais) | — (conflito aberto; ver afirmacións temporais) | Centro Cultural Marcos Valcárcel (adscrición do inventario) | MV | EX01-COMP-002: horas distintas e posible aprazamento, sen confirmar celebración. Afirmacións: TM-01–03. Non se escolle valor temporal canónico. | E4 §Centro Cultural Marcos Valcárcel, fila `MV-01`; E6 §Contraste por evento; incidencias en E4 |
| MV-02 | Punto y seguido | — (conflito aberto; ver afirmacións temporais) | — (conflito aberto; ver afirmacións temporais) | Centro Cultural Marcos Valcárcel (adscrición do inventario) | MV | EX01-COMP-010: datas distintas, mesma unidade. Afirmacións: TM-04–05. Non se escolle valor temporal canónico. | E4 §Centro Cultural Marcos Valcárcel, fila `MV-02`; E6 §Contraste por evento; incidencias en E4 |
| MV-03 | Carlos Ortega Bernabé: conferencia sobre as unidades de emerxencias internacionais da Cruz Vermella | — (conflito aberto; ver afirmacións temporais) | — (conflito aberto; ver afirmacións temporais) | Centro Cultural Marcos Valcárcel (adscrición do inventario) | MV | EX01-COMP-004: coincidencia centro/Press Club e discrepancia de Radio. Afirmacións: TM-06–08. Non se escolle valor temporal canónico. | E4 §Centro Cultural Marcos Valcárcel, fila `MV-03`; E6 §Contraste por evento; incidencias en E4 |
| MV-05 | I Xornada Internacional da Lonxevidade | 2026-11-07 | — | Centro Cultural Marcos Valcárcel (adscrición do inventario) | MV | Press Club relata 09:00–14:15 e programa detallado; non sumar partes. | E4 §Centro Cultural Marcos Valcárcel, fila `MV-05`; E6 §Contraste por evento; incidencias en E4 |
| MV-06 | Ciencia Calidade 2026 | 2026-11-07 | — | Centro Cultural Marcos Valcárcel (adscrición do inventario) | MV | Non fusionar coa Lonxevidade só por compartir centro e data. | E4 §Centro Cultural Marcos Valcárcel, fila `MV-06`; E6 §Contraste por evento; incidencias en E4 |
| MV-07 | Pateiro — El aprendiz de arquero | — (conflito aberto; ver afirmacións temporais) | — (conflito aberto; ver afirmacións temporais) | Centro Cultural Marcos Valcárcel (adscrición do inventario) | MV | EX01-COMP-001: intervalos distintos; listaxe/ficha do centro seguen sendo a mesma fonte. Afirmacións: TM-09–11. Non se escolle valor temporal canónico. | E4 §Centro Cultural Marcos Valcárcel, fila `MV-07`; E6 §Contraste por evento; incidencias en E4 |
| MV-08 | 31 OFF. Terra do Anel, unha viaxe entre reinos | 2026-09-17 | 2026-11-01 | Centro Cultural Marcos Valcárcel (adscrición do inventario) | MV | Exposición continuada; unha unidade. | E4 §Centro Cultural Marcos Valcárcel, fila `MV-08`; E6 §Contraste por evento; incidencias en E4 |
| MV-09 | Esteban Deláiglesia — Ecosistema dunha rodaxe | 2026-09-18 | 2026-11-01 | Centro Cultural Marcos Valcárcel (adscrición do inventario) | MV | Exposición continuada; unha unidade. | E4 §Centro Cultural Marcos Valcárcel, fila `MV-09`; E6 §Contraste por evento; incidencias en E4 |
| LR-01 | Nicolás Muller en Galicia | 2026-09-17 | 2027-01-09 | Afundación Ourense | LR | Exposición; visita guiada do 05/11 pendente de clasificación independente e non engadida. | E4 §Incorporacións provisionais identificadas en La Región, fila `LR-01`; E7 §§2–7 |
| LR-02 | LSYTSDA (Lo siento, yo tampoco soy de aquí) | 2026-09-24 | 2026-11-13 | Sala Alterarte, campus de Ourense | LR | Exposición continuada; unha unidade. | E4 §Incorporacións provisionais identificadas en La Región, fila `LR-02`; E7 §§2–7 |
| LR-03 | Judith Hill — O Gozo Festival | 2026-11-05 | — | Teatro Principal | LR | 20:00 segundo inventario; promoción de entradas en Press Club é a mesma actividade. | E4 §Incorporacións provisionais identificadas en La Región, fila `LR-03`; E7 §§2–7 |
| LR-04 | CatArte 2026: sesión do 5 de novembro | 2026-11-05 | — | Centro Cultural Marcos Valcárcel | LR | Só sesión do 05/11; outras sesións 12,19,26 fóra da xanela. Web e plataforma de venda sen identificar. Non localizado na axenda do centro consultada: non é ausencia confirmada. | E4 §Incorporacións provisionais identificadas en La Región, fila `LR-04`; E7 §§2–7 |
| LR-05 | A manipulación no xornalismo e na historia | — (conflito aberto; ver afirmacións temporais) | — (conflito aberto; ver afirmacións temporais) | Liceo de Ourense | LR | EX01-COMP-005: horas distintas; non resolver por maioría. Afirmacións: TM-12–14. Non se escolle valor temporal canónico. | E4 §Incorporacións provisionais identificadas en La Región, fila `LR-05`; E7 §§2–7 |
| LR-06 | A Auga na Historia II | 2026-10-29 | — | Facultade de Historia, campus de Ourense | LR | 09:50; xornada de tres intervencións, unha unidade. | E4 §Incorporacións provisionais identificadas en La Región, fila `LR-06`; E7 §§2–7 |
| LR-07 | A xoaniña que bebeu na folla — Fina Casalderrey | 2026-10-29 | — | Facultade de Educación e Traballo Social | LR | 18:00; só esta sesión do ciclo de outubro dentro da xanela. | E4 §Incorporacións provisionais identificadas en La Región, fila `LR-07`; E7 §§2–7 |
| MUS-01 | Concerto de jazz | 2026-10-29 | — | Café Latino | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-01` |
| MUS-02 | Jorge Gil | 2026-10-30 | — | Liceo | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-02` |
| MUS-03 | Alondra Bentley | 2026-10-30 | — | Café Pop Torgal | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-03` |
| MUS-04 | Amparo Sánchez | 2026-10-30 | — | Café Auriense | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-04` |
| MUS-05 | Fake Robotiqe + Robot City | 2026-10-30 | — | Café El Pueblo | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-05` |
| MUS-06 | Nugalha | 2026-10-30 | — | Antiga O’Renque | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-06` |
| MUS-07 | Pintas Acústicas | 2026-10-31 | — | O Moucho | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-07` |
| MUS-08 | World Brain | 2026-10-31 | — | Café Pop Torgal | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-08` |
| MUS-09 | Màbu | 2026-10-31 | — | Café Auriense | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-09` |
| MUS-10 | Ciudad Naranjo | 2026-10-31 | — | Café El Pueblo | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-10` |
| MUS-11 | Reservados Band | 2026-10-31 | — | Bar Papelón | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-11` |
| MUS-12 | Calcuta | 2026-11-04 | — | Café El Pueblo | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-12` |
| MUS-13 | Sara Hebe | 2026-11-05 | — | Café El Pueblo | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-13` |
| MUS-14 | Concerto de jazz | 2026-11-05 | — | Café Latino | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-14` |
| MUS-15 | Javier López Jorge | 2026-11-06 | — | Liceo | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-15` |
| MUS-16 | Dani Lança | 2026-11-06 | — | Café Auriense | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-16` |
| MUS-17 | Güru | 2026-11-07 | — | Café Trampitán | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-17` |
| MUS-18 | Stivijoes | 2026-11-07 | — | Café Pop Torgal | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-18` |
| MUS-19 | Urban Femme Fest | 2026-11-07 | — | Café Auriense | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-19` |
| MUS-20 | Carlos Campoy | 2026-11-07 | — | Ceres 1894 | MUS | H1; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-20` |
| MUS-21 | Begoña Mazaíra & Alex | 2026-11-08 | — | Liceo | MUS | H1/H2; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-21` |
| MUS-22 | Magosto Extremo | 2026-11-08 | — | Café El Pueblo | MUS | H1/H2; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-22` |
| MUS-23 | Concerto San Martiño: Coral do Liceo | 2026-11-10 | — | Liceo | MUS | H1/H2; ficha/confirmación directa por recuperar; fonte publicadora descoñecida salvo atribución expresa en B. | E8 §Actuacións musicais recuperadas do historial, `MUS-23` |
| AMP-01 | Tony Lane — Cruzando o mar intransitable | — | — | — | AMP | Exposición; faltan intervalo, espazo e evidencia individual; fonte publicadora descoñecida.; dato temporal relatado: Pendente. | E8 §Outras unidades recuperables e incompletas, `AMP-01` (U) |
| AMP-02 | Tamara Feijoo — El elemento caprichoso | — | — | Marisa Marimón | AMP | Non fixar fin; V3 publica 18/09–02/11; outra versión non recuperada; TM-15–16, sen datas canónicas.; dato temporal relatado: Fin discrepante. | E8 §Outras unidades recuperables e incompletas, `AMP-02` (U/V3) |
| AMP-03 | El extraño orden de las cosas | — | — | — | AMP | Faltan intervalo, espazo e evidencia individual; fonte publicadora descoñecida.; dato temporal relatado: Pendente. | E8 §Outras unidades recuperables e incompletas, `AMP-03` (U) |
| AMP-04 | Elvira Vaquero — Noemas | — | — | — | AMP | Faltan intervalo, espazo e evidencia individual; fonte publicadora descoñecida.; dato temporal relatado: Pendente. | E8 §Outras unidades recuperables e incompletas, `AMP-04` (U) |
| AMP-05 | XXXVI Exposición Filatélica San Martiño | 2026-11-09 | 2026-11-15 | Liceo | AMP | Anuncio visible; non proba celebración; dato temporal relatado: 09–15/11 (V2). | E8 §Outras unidades recuperables e incompletas, `AMP-05` (U/V2) |
| AMP-06 | Resurrection | 2026-11-02 | — | Casa da Cultura segundo V1 | AMP | Anuncio; non proba celebración; dato temporal relatado: 02/11. | E8 §Outras unidades recuperables e incompletas, `AMP-06` (U/V1) |
| AMP-07 | Vivir a terra | 2026-11-04 | — | Casa da Cultura segundo V1 | AMP | V1 escribe Vivira a terra; manter variante, non duplicar; dato temporal relatado: 04/11. | E8 §Outras unidades recuperables e incompletas, `AMP-07` (U/V1) |
| AMP-08 | Contratei un sicario | 2026-11-09 | — | — (sede individual pendente; Cineclube non se trata como sede) | AMP | Falta ficha específica accesible; dato temporal relatado: 09/11. | E8 §Outras unidades recuperables e incompletas, `AMP-08` (U) |
| AMP-09 | ¡Acojonado! — Miguel Miguel | 2026-11-06 | — | Teatro Principal | AMP | 20:00 Turismo / 20:30 Teatro; non resolver; dato temporal relatado: 06/11; hora discrepante. Ver B.2; non se adopta hora canónica. | E8 §Outras unidades recuperables e incompletas, `AMP-09` (U) |
| AMP-10 | Un matrimonio sin filtros | 2026-11-07 | — | Teatro Principal | AMP | Un espectáculo, dúas funcións; Turismo só 18:00; dato temporal relatado: 07/11; 18:00 e 20:00 segundo Teatro. Ver B.2; non se adopta hora canónica. | E8 §Outras unidades recuperables e incompletas, `AMP-10` (U) |
| AMP-11 | Arqueoloxía en monodose: A igrexa de Santalla de Esperante | 2026-11-02 | — | — (sede concreta pendente) | AMP | Programación MAPOU relatada; actividade independente, non sesión repetida; dato temporal relatado: 02/11. | E8 §Outras unidades recuperables e incompletas, `AMP-11` (U/C); E10 §§4–7 |
| AMP-12 | Arqueoloxía en monodose: A vila romana dos Escouredos | 2026-11-09 | — | — (sede concreta pendente) | AMP | Programación MAPOU relatada; actividade independente; hora non recuperada; dato temporal relatado: 09/11. | E8 §Outras unidades recuperables e incompletas, `AMP-12` (U/C); E10 §§4–7 |
| AMP-13 | Presentación da peza do mes: Cerámicas campaniformes da Portela da Moada | 2026-11-11 | — | — (sede concreta pendente) | AMP | Programación MAPOU relatada; independente da Peza do mes de outubro xa na base; dato temporal relatado: 11/11. | E8 §Outras unidades recuperables e incompletas, `AMP-13` (U/C); E10 §§4–7 |
| AMP-14 | O derradeiro Gimlet — Diego Ameixeiras | 2026-11-03 | — | Libraría Tanco, Ourense | AMP | Cartel revisado na conversa principal; participa Fran Alonso, director de Xerais; dato temporal relatado: 03/11,19:30. | E8 §Outras unidades recuperables e incompletas, `AMP-14` (U/C); E10 §§4–7 |
| AMP-15 | Escoitando comunidades que se coidan: VII Encontro arredor do rural | 2026-10-30 | — | Edificio de Ferro, Campus de Ourense | AMP | Contraste institucional UVigo relatado; non repetido nesta sesión; dato temporal relatado: 30/10,10:00. | E8 §Outras unidades recuperables e incompletas, `AMP-15` (U/C); E10 §§4–7 |
| AMP-16 | Goma de borrar — Valeria G. Caneda | 2026-10-30 | — | Espazo Lector Nobel | AMP | Non duplicar como obradoiro por aparecer no mesmo local; dato temporal relatado: 30/10, 19:30 (H3). | E8 §Outras unidades recuperables e incompletas, `AMP-16` (U/H3) |
| AMP-17 | Indie Pop Británico dos anos 80 | 2026-10-29 | — | Café Pop Torgal | AMP | Charla-audición confirmada na investigación; distinta dos concertos; dato temporal relatado: 29/10,20:30. | E8 §Outras unidades recuperables e incompletas, `AMP-17` (U/C); E10 §§4–7 |
| AMP-18 | Ourense na Túa Memoria: Recunchos — Cine | 2026-11-09 | — | Liceo de Ourense | AMP | Café-faladoiro; proxecto Recunchos da Nosa Memoria; Liceo e Salubrízate; discrepancia conservada; dato temporal relatado: 09/11;16:30 provisional /19:30 Turismo. Ver B.2; non se adopta hora canónica. | E8 §Outras unidades recuperables e incompletas, `AMP-18` (U/V2/C); E10 §§4–7 |
| AMP-19 | II Ciclo de Cine: Tempos de feminismo en plano secuencia | 2026-11-05 | — | Aula magna do Edificio Xurídico-Empresarial, Campus de Ourense | AMP | Organiza Facultade de Relacións Internacionais da UVigo; un composto, programa abaixo; dato temporal relatado: 05/11,13:00–21:00. | E8 §Outras unidades recuperables e incompletas, `AMP-19` (U/H0/C); E10 §§4–7 |
| AMP-20 | Taller infantil Samaín | 2026-10-31 | — | Pita na Uralita | AMP | Unidade independente aceptada; compartir temática non a integra automaticamente no Samaín municipal; dato temporal relatado: 31/10. | E8 §Outras unidades recuperables e incompletas, `AMP-20` (U/H3/C) |
| AMP-21 | Crea tus wax melts otoñales | 2026-10-31 | — | Estudio Riquiño | AMP | Anuncio recuperado; falta referencia primaria; dato temporal relatado: 31/10, 17:00. | E8 §Outras unidades recuperables e incompletas, `AMP-21` (U/H3) |
| AMP-22 | La abuela de Grúfalo | 2026-10-31 | — | Espazo Lector Nobel | AMP | Título recuperado; non inferir formato só polo bloque de obradoiros; dato temporal relatado: 31/10, 11:00. | E8 §Outras unidades recuperables e incompletas, `AMP-22` (U/H3) |
| AMP-23 | Pumpkin Carving | 2026-10-31 | — | Cafetería Forasteiro | AMP | Unidade independente de AMP-24 e FOR-03; non programa composto único; dato temporal relatado: 31/10,16:00–17:00. | E8 §Outras unidades recuperables e incompletas, `AMP-23` (U/H3/C) |
| AMP-24 | Conecta con los animales, conecta contigo | 2026-11-06 | — | Cafetería Forasteiro | AMP | Unidade independente aceptada na investigación; evidencia primaria pendente de arquivo; dato temporal relatado: 06/11,17:00. | E8 §Outras unidades recuperables e incompletas, `AMP-24` (U/H3/C) |
| AMP-25 | Flores en el arte | 2026-11-06 | 2026-11-07 | Estudio Ana Navas | AMP | Unha actividade con dúas sesións; cartel revisado na conversa principal; dato temporal relatado: 06/11,19:00;07/11,17:30. Inicio/fin delimitan sesións, non actividade continua. | E8 §Outras unidades recuperables e incompletas, `AMP-25` (U/C); E10 §§4–7 |
| AMP-26 | Xogos de mesa para maiores de 60 anos | 2026-11-05 | — | Biblioteca Pública Nós, sala xuvenil | AMP | Xogos contemporáneos; gratuíta con inscrición; distinta de Alba Polo; sesión 19/11 fóra da xanela; dato temporal relatado: 05/11,11:00–12:30. | E8 §Outras unidades recuperables e incompletas, `AMP-26` (U/C); E10 §§4–7 |
| AMP-27 | Máis alá do volante: descubrindo o automobilismo | 2026-11-06 | — | Ponte Vella, segunda planta | AMP | Divulgación deportiva e técnica; Mario Rivera e Rodrigo González; charla, simulador, material e sorteo son compoñentes; dato temporal relatado: 06/11,17:15. | E8 §Outras unidades recuperables e incompletas, `AMP-27` (U/C); E10 §§4–7 |
| AMP-28 | Feria de la Chinita Galicia | 2026-11-08 | — | Campo da Feira, Ourense | AMP | Un composto cultural venezolano con música, gastronomía e comunidade; perfil identificado abaixo; dato temporal relatado: 08/11,12:00. | E8 §Outras unidades recuperables e incompletas, `AMP-28` (U/H2/C); E10 §§4–7 |
| AMP-29 | Festa do Magosto de Ourense 2026 | 2026-11-07 | 2026-11-11 | Sala Ánxel Valente e Praza Maior/Alameda; programa abaixo | AMP | Un composto segundo a agrupación do Concello; non sumar partes; dato temporal relatado: 07/11 e 11/11. Inicio/fin delimitan sesións, non actividade continua. | E8 §Outras unidades recuperables e incompletas, `AMP-29` (U/C); E10 §§4–7 |
| PV-01 | Figuras de la pandilla Halloween | 2026-10-29 | 2026-10-30 | Ponte Vella | PV | Unha actividade creativa infantil con varias sesións; C, carteis revisados na conversa principal; sesións/horas relatadas: 29 e 30/10. Inicio/fin delimitan sesións, non actividade continua. | E8 §Cinco unidades omitidas, `PV-01`; E10 §2 |
| PV-02 | Mundos en miniatura Halloween | 2026-10-31 | — | Ponte Vella | PV | Actividade creativa infantil independente; C; sesións/horas relatadas: 31/10. | E8 §Cinco unidades omitidas, `PV-02`; E10 §2 |
| PV-03 | Mago José Rivera | 2026-10-31 | — | Ponte Vella | PV | Espectáculo de maxia independente; C; sesións/horas relatadas: 31/10,19:00. | E8 §Cinco unidades omitidas, `PV-03`; E10 §2 |
| PV-04 | Dibujo y pintura con Leandro Sánchez | 2026-10-30 | 2026-11-07 | Ponte Vella | PV | Unha actividade artística con catro sesións; C; sesións/horas relatadas: 30 e 31/10;06 e 07/11. Inicio/fin delimitan sesións, non actividade continua. | E8 §Cinco unidades omitidas, `PV-04`; E10 §2 |
| FOR-03 | Principios de Ikebana | 2026-11-07 | — | Cafetería Forasteiro | FOR | Unidade independente de arte floral xaponesa; C, publicación do establecemento en Instagram revisada na investigación; sesións/horas relatadas: 07/11,16:00. | E8 §Cinco unidades omitidas, `FOR-03`; E10 §3 |

## B. Atribucións evento–fonte e soporte evidencial

### B.1. Vocabulario e dispoñibilidade

Os campos separan **attribution_status**, **evidence_type** e **evidence_availability**. Os IDs AT-01–47 engádense só para reconciliar, na mesma orde, as 47 liñas da primeira versión; non son novos eventos nin publicacións inventadas. A cada atribución correspóndelle polo momento un rexistro de soporte, que pode citar varios documentos.

| Dimensión | Valores e criterio |
| --- | --- |
| attribution_status | Confirmada documentalmente: asociación expresa evento–fonte nos documentos. Probable: indicio explícito aínda non confirmado. Pendente de identificación ou contraste: fonte ou comprobación incompleta. |
| evidence_type | Contido primario conservado: payload orixinal arquivado. Comprobación anterior relatada na documentación: atribución/observación previa rexistrada, sen converter a consulta anterior nunha consulta actual. Indicio documentado: só se existise un indicio concreto; non se emprega aquí. |
| evidence_availability | Contido orixinal conservado; Referencia ou URL dispoñible, sen contido arquivado; Referencia documental a unha comprobación anterior; Evidencia primaria non localizada. Esta última etiqueta nas dúas CatArte refírese ao expediente dispoñible, non a unha conclusión de inexistencia da publicación. |
| source_id e pending_source | Coñecida: ID do catálogo e etiqueta pendente baleira. Anónima: ID baleiro e descrición da publicación mencionada. Non se crea un ID ficticio. |
| consultation_date | Só a data explicitamente documentada da comprobación, non a data do evento, do documento ou da creación desta matriz. E2 sitúa a comprobación Xunta o 28/10; E8 V1/V2/V3 identifican as consultas de Radio, Liceo e Turismo o 02/11. Nas demais, —. |
| specific_url | Só a URL individual xa conservada. As URL xerais das axendas constan nas referencias E e non se presentan como ligazón específica dun evento. |

**Confirmada documentalmente non significa evidencia primaria dispoñible, verificación recente, data correcta nin celebración efectiva.** A condición de acceso tampouco determina a inclusión. Non se infiren novas fontes por compartir sede.

| attribution_id | event_id | source_id | pending_source | attribution_status | evidence_type | evidence_availability | evidence_reference | specific_url | consultation_date | notes |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| AT-01 | 157064 | SRC-XUNTA | — | Confirmada documentalmente | Contido primario conservado | Contido orixinal conservado | E1 `listaAxenda[id=157064]` | https://www.cultura.gal/gl/evento/128578/69/157064 | 2026-10-28 | Payload da fonte conservado; non implica segunda fonte nin celebración efectiva. Data de comprobación explicitada en E2; non é a data do evento nin un rexistro HTTP. |
| AT-02 | 157066 | SRC-XUNTA | — | Confirmada documentalmente | Contido primario conservado | Contido orixinal conservado | E1 `listaAxenda[id=157066]` | https://www.cultura.gal/gl/evento/128580/69/157066 | 2026-10-28 | Payload da fonte conservado; non implica segunda fonte nin celebración efectiva. Data de comprobación explicitada en E2; non é a data do evento nin un rexistro HTTP. |
| AT-03 | 156460 | SRC-XUNTA | — | Confirmada documentalmente | Contido primario conservado | Contido orixinal conservado | E1 `listaAxenda[id=156460]` | https://www.cultura.gal/gl/evento/127892/13/156460 | 2026-10-28 | Payload da fonte conservado; non implica segunda fonte nin celebración efectiva. Data de comprobación explicitada en E2; non é a data do evento nin un rexistro HTTP. |
| AT-04 | 157005 | SRC-XUNTA | — | Confirmada documentalmente | Contido primario conservado | Contido orixinal conservado | E1 `listaAxenda[id=157005]` | https://www.cultura.gal/gl/evento/128509/21/157005 | 2026-10-28 | Payload da fonte conservado; non implica segunda fonte nin celebración efectiva. Data de comprobación explicitada en E2; non é a data do evento nin un rexistro HTTP. |
| AT-05 | 157020 | SRC-XUNTA | — | Confirmada documentalmente | Contido primario conservado | Contido orixinal conservado | E1 `listaAxenda[id=157020]` | https://www.cultura.gal/gl/evento/128530/70/157020 | 2026-10-28 | Payload da fonte conservado; non implica segunda fonte nin celebración efectiva. Data de comprobación explicitada en E2; non é a data do evento nin un rexistro HTTP. |
| AT-06 | 157007 | SRC-XUNTA | — | Confirmada documentalmente | Contido primario conservado | Contido orixinal conservado | E1 `listaAxenda[id=157007]` | https://www.cultura.gal/gl/evento/128511/70/157007 | 2026-10-28 | Payload da fonte conservado; non implica segunda fonte nin celebración efectiva. Data de comprobación explicitada en E2; non é a data do evento nin un rexistro HTTP. |
| AT-07 | 157095 | SRC-XUNTA | — | Confirmada documentalmente | Contido primario conservado | Contido orixinal conservado | E1 `listaAxenda[id=157095]` | https://www.cultura.gal/gl/evento/128623/22/157095 | 2026-10-28 | Payload da fonte conservado; non implica segunda fonte nin celebración efectiva. Data de comprobación explicitada en E2; non é a data do evento nin un rexistro HTTP. |
| AT-08 | 157018 | SRC-XUNTA | — | Confirmada documentalmente | Contido primario conservado | Contido orixinal conservado | E1 `listaAxenda[id=157018]` | https://www.cultura.gal/gl/evento/128528/2/157018 | 2026-10-28 | Payload da fonte conservado; non implica segunda fonte nin celebración efectiva. Data de comprobación explicitada en E2; non é a data do evento nin un rexistro HTTP. |
| AT-09 | 157319 | SRC-XUNTA | — | Confirmada documentalmente | Contido primario conservado | Contido orixinal conservado | E1 `listaAxenda[id=157319]` | https://www.cultura.gal/gl/evento/128902/13/157319 | 2026-10-28 | Payload da fonte conservado; non implica segunda fonte nin celebración efectiva. Data de comprobación explicitada en E2; non é a data do evento nin un rexistro HTTP. |
| AT-10 | 157321 | SRC-XUNTA | — | Confirmada documentalmente | Contido primario conservado | Contido orixinal conservado | E1 `listaAxenda[id=157321]` | https://www.cultura.gal/gl/evento/128904/21/157321 | 2026-10-28 | Payload da fonte conservado; non implica segunda fonte nin celebración efectiva. Data de comprobación explicitada en E2; non é a data do evento nin un rexistro HTTP. |
| AT-11 | 157333 | SRC-XUNTA | — | Confirmada documentalmente | Contido primario conservado | Contido orixinal conservado | E1 `listaAxenda[id=157333]` | https://www.cultura.gal/gl/evento/128920/70/157333 | 2026-10-28 | Payload da fonte conservado; non implica segunda fonte nin celebración efectiva. Data de comprobación explicitada en E2; non é a data do evento nin un rexistro HTTP. |
| AT-12 | 157323 | SRC-XUNTA | — | Confirmada documentalmente | Contido primario conservado | Contido orixinal conservado | E1 `listaAxenda[id=157323]` | https://www.cultura.gal/gl/evento/128906/21/157323 | 2026-10-28 | Payload da fonte conservado; non implica segunda fonte nin celebración efectiva. Data de comprobación explicitada en E2; non é a data do evento nin un rexistro HTTP. |
| AT-13 | MUN-01 | SRC-CONCELLO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Concello de Ourense, `MUN-01`; E5 §5 | — | — | Revisión manual relatada. URL xeral na sección; ficha individual non inventariada. |
| AT-14 | MUN-02 | SRC-CONCELLO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Concello de Ourense, `MUN-02`; E5 §5 | — | — | Revisión manual relatada. URL xeral na sección; ficha individual non inventariada. |
| AT-15 | MUN-03 | SRC-CONCELLO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Concello de Ourense, `MUN-03`; E5 §5 | — | — | Revisión manual relatada. URL xeral na sección; ficha individual non inventariada. |
| AT-16 | MUN-06 | SRC-CONCELLO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Concello de Ourense, `MUN-06`; E5 §5 | — | — | Revisión manual relatada. URL xeral na sección; ficha individual non inventariada. |
| AT-17 | MUN-07 | SRC-CONCELLO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Concello de Ourense, `MUN-07`; E5 §5 | — | — | Revisión manual relatada. URL xeral na sección; ficha individual non inventariada. |
| AT-18 | MV-01 | SRC-MV | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Centro Cultural Marcos Valcárcel, `MV-01`; E5 §6; E6 | — | — | Atribución á axenda do centro, distinta da adscrición como sede. Orixinal individual pendente de arquivo. |
| AT-19 | MV-02 | SRC-MV | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Centro Cultural Marcos Valcárcel, `MV-02`; E5 §6; E6 | — | — | Atribución á axenda do centro, distinta da adscrición como sede. Orixinal individual pendente de arquivo. |
| AT-20 | MV-03 | SRC-MV | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Centro Cultural Marcos Valcárcel, `MV-03`; E5 §6; E6 | — | — | Atribución á axenda do centro, distinta da adscrición como sede. Orixinal individual pendente de arquivo. |
| AT-21 | MV-05 | SRC-MV | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Centro Cultural Marcos Valcárcel, `MV-05`; E5 §6; E6 | — | — | Atribución á axenda do centro, distinta da adscrición como sede. Orixinal individual pendente de arquivo. |
| AT-22 | MV-06 | SRC-MV | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Centro Cultural Marcos Valcárcel, `MV-06`; E5 §6; E6 | — | — | Atribución á axenda do centro, distinta da adscrición como sede. Orixinal individual pendente de arquivo. |
| AT-23 | MV-07 | SRC-MV | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia ou URL dispoñible, sen contido arquivado | E4 §Centro Cultural Marcos Valcárcel, `MV-07`; E5 §6; E6 | https://www.centroculturaldeourense.com/exposicions/el-aprendiz-de-arquero | — | Atribución á axenda do centro, distinta da adscrición como sede. URL de ficha en E4: https://www.centroculturaldeourense.com/exposicions/el-aprendiz-de-arquero; conservala non arquiva o seu contido. |
| AT-24 | MV-08 | SRC-MV | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Centro Cultural Marcos Valcárcel, `MV-08`; E5 §6; E6 | — | — | Atribución á axenda do centro, distinta da adscrición como sede. Orixinal individual pendente de arquivo. |
| AT-25 | MV-09 | SRC-MV | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Centro Cultural Marcos Valcárcel, `MV-09`; E5 §6; E6 | — | — | Atribución á axenda do centro, distinta da adscrición como sede. Orixinal individual pendente de arquivo. |
| AT-26 | LR-01 | SRC-LAREGION | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Incorporacións provisionais identificadas en La Región, `LR-01`; E7 §2 | — | — | Canle individual non inventariada. |
| AT-27 | LR-02 | SRC-LAREGION | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Incorporacións provisionais identificadas en La Región, `LR-02`; E7 §2 | — | — | Canle individual non inventariada. |
| AT-28 | LR-03 | SRC-LAREGION | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Incorporacións provisionais identificadas en La Región, `LR-03`; E7 §2 | — | — | Canle individual non inventariada. |
| AT-29 | LR-04 | SRC-LAREGION | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Incorporacións provisionais identificadas en La Región, `LR-04`; E7 §2 | — | — | Canle individual non inventariada. |
| AT-30 | LR-05 | SRC-LAREGION | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Incorporacións provisionais identificadas en La Región, `LR-05`; E7 §2 | — | — | Artigo de axenda diaria identificado en E4 EX01-COMP-005; hora 20:00 fronte a 19:30 noutras fontes. |
| AT-31 | LR-06 | SRC-LAREGION | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Incorporacións provisionais identificadas en La Región, `LR-06`; E7 §2 | — | — | Canle individual non inventariada. |
| AT-32 | LR-07 | SRC-LAREGION | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Incorporacións provisionais identificadas en La Región, `LR-07`; E7 §2 | — | — | Canle individual non inventariada. |
| AT-33 | MUN-01 | SRC-LAREGION | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Outros candidatos examinados en La Región; E7 §4 | — | — | Título en castelán identificado como o mesmo evento da aviación. |
| AT-34 | MV-07 | SRC-LAREGION | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §La Región e Press Club; E7 §6 | — | — | Exposición coincidente co centro; non é un novo evento. Conservar datas discrepantes de EX01-COMP-001. |
| AT-35 | MV-08 | SRC-LAREGION | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §La Región e Press Club; E7 §6 | — | — | Exposición coincidente co centro; non é un novo evento. |
| AT-36 | MV-09 | SRC-LAREGION | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §La Región e Press Club; E7 §6 | — | — | Exposición coincidente co centro; non é un novo evento. |
| AT-37 | MV-01 | SRC-PRESSCLUB | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Press Club: coincidencias identificadas e alcance da revisión; E7 §5 | — | — | Mesmo evento; discrepancia horaria e posible aprazamento, non resoltos. |
| AT-38 | MV-03 | SRC-PRESSCLUB | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Press Club: coincidencias identificadas e alcance da revisión; E7 §5 | — | — | Mesmo evento;19:45 coincide coa axenda do centro. |
| AT-39 | MV-05 | SRC-PRESSCLUB | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Press Club: coincidencias identificadas e alcance da revisión; E7 §5 | — | — | Programa máis detallado;09:00–14:15. |
| AT-40 | LR-03 | SRC-PRESSCLUB | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Press Club: coincidencias identificadas e alcance da revisión; E7 §5 | — | — | Promoción de entradas do mesmo concerto, non evento distinto. |
| AT-41 | MV-02 | SRC-TURISMO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 §Incidencias da ampliación, EX01-COMP-010 | — | — | Turismo 10/11 / centro 04/11; identidade compartida relatada, data non resolta. |
| AT-42 | MV-03 | SRC-RADIOLIVERDADE | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 EX01-COMP-004; E8 §Fontes e comprobacións limitadas (V1) | — | 2026-11-02 | Observación directa anterior rexistrada no caderno, sen payload individual arquivado aquí;05/11 ás19:30. Clasificada como relato desta comprobación, non como nova consulta. Data da observación explicitada en E8 V1; non se repite a consulta. |
| AT-43 | LR-04 | SRC-TURISMO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 EX01-COMP-006; E7 §7 | — | — | Publicación coincidente relatada; URL individual pendente. |
| AT-44 | LR-04 | — | web específica de CatArte | Pendente de identificación ou contraste | Comprobación anterior relatada na documentación | Evidencia primaria non localizada | E4 EX01-COMP-006; E7 §7 | — | — | A publicación é mencionada, pero faltan identidade e URL da web. Liña de atribución incompleta, non unha fonte identificada. |
| AT-45 | LR-04 | — | plataforma de venda de CatArte | Pendente de identificación ou contraste | Comprobación anterior relatada na documentación | Evidencia primaria non localizada | E4 EX01-COMP-006; E7 §7 | — | — | Plataforma e URL non identificadas. Non inventar nome; non confundir publicación de venda con evento separado. |
| AT-46 | LR-05 | SRC-TURISMO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 EX01-COMP-005; E7 §7 | — | — | Publica19:30 segundo a revisión relatada; non se escolle hora correcta por maioría. |
| AT-47 | LR-05 | SRC-LICEO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 EX01-COMP-005; E7 §7 | — | — | Fonte publicadora explicitamente mencionada, ademais de ser a sede. 19:30; URL individual pendente. |
| AT-48 | MUS-15 | SRC-LICEO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E8 §Fontes e comprobacións limitadas, V2; fila `MUS-15` | — | 2026-11-02 | Comprobación previa relatada; orixinal non arquivado; non proba celebración efectiva. |
| AT-49 | MUS-21 | SRC-LICEO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E8 §Fontes e comprobacións limitadas, V2; fila `MUS-21` | — | 2026-11-02 | Comprobación previa relatada; orixinal non arquivado; non proba celebración efectiva. |
| AT-50 | MUS-23 | SRC-LICEO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E8 §Fontes e comprobacións limitadas, V2; fila `MUS-23` | — | 2026-11-02 | Comprobación previa relatada; orixinal non arquivado; non proba celebración efectiva. |
| AT-51 | AMP-05 | SRC-LICEO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E8 §Fontes e comprobacións limitadas, V2; fila `AMP-05` | — | 2026-11-02 | Comprobación previa relatada; orixinal non arquivado; non proba celebración efectiva. |
| AT-52 | AMP-02 | SRC-TURISMO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E8 V3; E4 EX01-COMP-015 | — | 2026-11-02 | Versión 18/09–02/11; alternativa non recuperada; non resolver. |
| AT-53 | AMP-06 | SRC-CINECLUBE | — | Probable | Indicio documentado | Referencia documental a unha comprobación anterior | E8 fila `AMP-06` e §Fontes e comprobacións limitadas, Cineclube | — | — | Indicio: filme asociado ao Cineclube e blog identificado como canle; a portada xeral non acredita esta publicación individual. Recuperar ficha antes de confirmar. |
| AT-54 | AMP-07 | SRC-CINECLUBE | — | Probable | Indicio documentado | Referencia documental a unha comprobación anterior | E8 fila `AMP-07` e §Fontes e comprobacións limitadas, Cineclube | — | — | Indicio: filme asociado ao Cineclube e blog identificado como canle; a portada xeral non acredita esta publicación individual. Recuperar ficha antes de confirmar. |
| AT-55 | AMP-08 | SRC-CINECLUBE | — | Probable | Indicio documentado | Referencia documental a unha comprobación anterior | E8 fila `AMP-08` e §Fontes e comprobacións limitadas, Cineclube | — | — | Indicio: filme asociado ao Cineclube e blog identificado como canle; a portada xeral non acredita esta publicación individual. Recuperar ficha antes de confirmar. |
| AT-56 | AMP-06 | SRC-RADIOLIVERDADE | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E8 V1 e fila `AMP-06` | — | 2026-11-02 | Anuncio observado anteriormente; AMP-07 coa variante Vivira a terra; non novo evento. |
| AT-57 | AMP-07 | SRC-RADIOLIVERDADE | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E8 V1 e fila `AMP-07` | — | 2026-11-02 | Anuncio observado anteriormente; AMP-07 coa variante Vivira a terra; non novo evento. |
| AT-58 | AMP-09 | SRC-TURISMO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 EX01-COMP-012; E8 fila `AMP-09`; E10 §7 | — | — | Publicación expresamente atribuída; conservar versións de horario en B.2. |
| AT-59 | AMP-09 | SRC-TEATRO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 EX01-COMP-012; E8 fila `AMP-09`; E10 §7 | — | — | Publicación expresamente atribuída; conservar versións de horario en B.2. |
| AT-60 | AMP-10 | SRC-TURISMO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 EX01-COMP-013; E8 fila `AMP-10`; E10 §7 | — | — | Publicación expresamente atribuída; conservar versións de horario en B.2. |
| AT-61 | AMP-10 | SRC-TEATRO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 EX01-COMP-013; E8 fila `AMP-10`; E10 §7 | — | — | Publicación expresamente atribuída; conservar versións de horario en B.2. |
| AT-62 | AMP-11 | SRC-MAPOU | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E10 §4, `AMP-11`; E8 fila correspondente | — | — | Programación do MAPOU expresamente identificada como fonte utilizada; non é atribución por sede. |
| AT-63 | AMP-12 | SRC-MAPOU | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E10 §4, `AMP-12`; E8 fila correspondente | — | — | Programación do MAPOU expresamente identificada como fonte utilizada; non é atribución por sede. |
| AT-64 | AMP-13 | SRC-MAPOU | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E10 §4, `AMP-13`; E8 fila correspondente | — | — | Programación do MAPOU expresamente identificada como fonte utilizada; non é atribución por sede. |
| AT-65 | AMP-14 | — | Cartel de O derradeiro Gimlet, emisor sen identificar | Pendente de identificación ou contraste | Comprobación anterior relatada na documentación | Evidencia primaria non localizada | E10 §5, AMP-14; E8 §Datos e evidencias aínda pendentes | — | — | Cartel revisado relatado; non asignar publicador Tanco ou Xerais a partir da sede ou participantes. |
| AT-66 | AMP-15 | SRC-UVIGO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E10 §5, AMP-15; E8 AMP-15 | — | — | Axenda e información institucional expresamente citadas; URL xeral en E8; consulta específica sen data. |
| AT-67 | AMP-18 | SRC-TURISMO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E4 EX01-COMP-011; E10 §5, AMP-18 | — | — | Publicación ás 19:30; non adopción dunha hora correcta. |
| AT-68 | AMP-18 | SRC-LICEO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E8 V2; E10 §5, AMP-18 | — | 2026-11-02 | Programación ás 16:30; tamén se relata cartel coa mesma hora. |
| AT-69 | AMP-19 | SRC-FRRII | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia ou URL dispoñible, sen contido arquivado | E10 §5, AMP-19; E8 §Fontes e comprobacións limitadas | https://frrii.uvigo.es/gl/actualidade/eventos/ii-ciclo-de-cine-tempos-de-feminismo-en-plano-secuencia | — | URL do programa recibido; acceso anterior bloqueado. Non nova comprobación directa. |
| AT-70 | AMP-25 | — | Cartel de Flores en el arte, emisor sen identificar | Pendente de identificación ou contraste | Comprobación anterior relatada na documentación | Evidencia primaria non localizada | E10 §5, AMP-25; E8 fila correspondente | — | — | Cartel compartido; Ana Navas é espazo indicado, non fonte publicadora confirmada por dedución. |
| AT-71 | AMP-28 | SRC-CHINITA-IG | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E10 §5, AMP-28; E8 §Fontes e comprobacións limitadas | — | — | Perfil identificado; publicación específica e data de consulta non recuperadas. |
| AT-72 | AMP-29 | SRC-CONCELLO | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia ou URL dispoñible, sen contido arquivado | E10 §5, AMP-29; E8 §Programación interna conservada | https://ourense.gal/gl/evento/festa-do-magosto-de-ourense-2026-festa-de-interese-turistico | — | Un composto; URL recibida, acceso anterior bloqueado; programa relatado. |
| AT-73 | PV-01 | SRC-PONTEVELLA | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E10 §2, `PV-01`; E8 §Cinco unidades omitidas | — | — | A procedencia dos carteis atribúese expresamente a Ponte Vella; non se conserva o orixinal nin unha URL. |
| AT-74 | PV-02 | SRC-PONTEVELLA | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E10 §2, `PV-02`; E8 §Cinco unidades omitidas | — | — | A procedencia dos carteis atribúese expresamente a Ponte Vella; non se conserva o orixinal nin unha URL. |
| AT-75 | PV-03 | SRC-PONTEVELLA | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E10 §2, `PV-03`; E8 §Cinco unidades omitidas | — | — | A procedencia dos carteis atribúese expresamente a Ponte Vella; non se conserva o orixinal nin unha URL. |
| AT-76 | PV-04 | SRC-PONTEVELLA | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E10 §2, `PV-04`; E8 §Cinco unidades omitidas | — | — | A procedencia dos carteis atribúese expresamente a Ponte Vella; non se conserva o orixinal nin unha URL. |
| AT-77 | FOR-03 | SRC-FORASTEIRO-IG | — | Confirmada documentalmente | Comprobación anterior relatada na documentación | Referencia documental a unha comprobación anterior | E10 §3, FOR-03; E8 §Cinco unidades omitidas | — | — | Publicación do establecemento en Instagram expresamente relatada; URL do post non recuperada. |

### B.2. Afirmacións temporais conflitivas ou información de sesións incompleta

Unha afirmación é unha versión publicada ou relatada, non outra unidade de evento nin unha relación nova de cobertura. `start_date/start_time/end_date/end_time` transcriben **valores afirmados pola fonte**, non valores canónicos. Mantéñense intactas TM-01–14 do piloto. As afirmacións novas conservan tamén información de funcións incompleta (AMP-10), que non é por si soa unha contradición horaria. Non se enchen horas finais nin se interpreta a ausencia dun fin como duración cero.

As versións coincidentes non se impoñen por maioría. As superficies distintas dunha fonte non crean outra atribución. As referencias sen fonte identificada ao aprazamento e ao fin alternativo non crean unha fonte no catálogo. Todas estas afirmacións son comprobacións anteriores relatadas en E4/E7/E8/E10, non contido primario arquivado. A táboa non demostra o estado actual nin a celebración efectiva dos eventos.

| assertion_id | event_id | source_id | surface_or_pending_source | start_date | start_time | end_date | end_time | state_or_limit | evidence_reference | specific_url | consultation_date |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| TM-01 | MV-01 | SRC-MV | Axenda do centro | 2026-10-29 | 20:15 | — | — | Anuncio relatado; celebración non confirmada | E4 EX01-COMP-002 | — | — |
| TM-02 | MV-01 | SRC-PRESSCLUB | Press Club | 2026-10-29 | 19:45 | — | — | Anuncio relatado; celebración non confirmada | E4 EX01-COMP-002; E7 §6 | — | — |
| TM-03 | MV-01 | — | Referencia posterior non identificada | — | — | — | — | Posible aprazamento; publicación e data por recuperar | E4 EX01-COMP-002 / Incidencias da ampliación; non unha fonte nova identificada | — | — |
| TM-04 | MV-02 | SRC-MV | Axenda do centro | 2026-11-04 | — | — | — | Versión relatada; conflito aberto | E4 Centro Cultural Marcos Valcárcel e EX01-COMP-010 | — | — |
| TM-05 | MV-02 | SRC-TURISMO | Axenda de Turismo | 2026-11-10 | — | — | — | Versión relatada; conflito aberto | E4 EX01-COMP-010 | — | — |
| TM-06 | MV-03 | SRC-MV | Axenda do centro | 2026-11-05 | 19:45 | — | — | Coincide con Press Club; conflito con Radio | E4 EX01-COMP-004; E7 §6 | — | — |
| TM-07 | MV-03 | SRC-PRESSCLUB | Press Club | 2026-11-05 | 19:45 | — | — | Coincide co centro; conflito con Radio | E4 EX01-COMP-004; E7 §6 | — | — |
| TM-08 | MV-03 | SRC-RADIOLIVERDADE | Axenda de Radio | 2026-11-05 | 19:30 | — | — | Observación anterior rexistrada; conflito aberto | E4 EX01-COMP-004; E8 V1 | — | 2026-11-02 |
| TM-09 | MV-07 | SRC-MV | Listaxe do centro | 2026-10-07 | — | 2026-11-08 | — | Intervalo publicado; non seleccionado | E4 EX01-COMP-001 | — | — |
| TM-10 | MV-07 | SRC-MV | Ficha individual do centro | 2026-10-08 | — | 2026-11-01 | — | Intervalo publicado; non seleccionado | E4 EX01-COMP-001 | https://www.centroculturaldeourense.com/exposicions/el-aprendiz-de-arquero | — |
| TM-11 | MV-07 | SRC-LAREGION | Listaxe/ficha de La Región segundo o relato | 2026-10-08 | — | 2026-11-01 | — | Intervalo publicado; non seleccionado | E4 EX01-COMP-001; E7 §6 | — | — |
| TM-12 | LR-05 | SRC-LAREGION | Artigo de axenda diaria | 2026-10-29 | 20:00 | — | — | Conflito horario aberto | E4 EX01-COMP-005; E7 §7 | — | — |
| TM-13 | LR-05 | SRC-LICEO | Axenda do Liceo | 2026-10-29 | 19:30 | — | — | Conflito horario aberto | E4 EX01-COMP-005; E7 §7 | — | — |
| TM-14 | LR-05 | SRC-TURISMO | Axenda de Turismo | 2026-10-29 | 19:30 | — | — | Conflito horario aberto | E4 EX01-COMP-005; E7 §7 | — | — |
| TM-15 | AMP-02 | SRC-TURISMO | Axenda de outubro | 2026-09-18 | — | 2026-11-02 | — | Versión recuperada; non se selecciona fin canónico | E8 V3; E4 EX01-COMP-015 | — | 2026-11-02 |
| TM-16 | AMP-02 | — | Versión alternativa non recuperada | — | — | — | — | Discrepancia relatada; valor e publicador descoñecidos, non se inventan | E4 EX01-COMP-015; E10 §7 | — | — |
| TM-17 | AMP-09 | SRC-TURISMO | Programación/axenda relatada | 2026-11-06 | 20:00 | — | — | Conflito horario aberto | E4 EX01-COMP-012; E10 §7 | — | — |
| TM-18 | AMP-09 | SRC-TEATRO | Programación/axenda relatada | 2026-11-06 | 20:30 | — | — | Conflito horario aberto | E4 EX01-COMP-012; E10 §7 | — | — |
| TM-19 | AMP-10 | SRC-TURISMO | Función anunciada | 2026-11-07 | 18:00 | — | — | Un espectáculo; Turismo recolle só unha das dúas funcións, non contradición da de 18:00 | E4 EX01-COMP-013; E10 §7 | — | — |
| TM-20 | AMP-10 | SRC-TEATRO | Función anunciada | 2026-11-07 | 18:00 | — | — | Un espectáculo; Turismo recolle só unha das dúas funcións, non contradición da de 18:00 | E4 EX01-COMP-013; E10 §7 | — | — |
| TM-21 | AMP-10 | SRC-TEATRO | Función anunciada | 2026-11-07 | 20:00 | — | — | Un espectáculo; Turismo recolle só unha das dúas funcións, non contradición da de 18:00 | E4 EX01-COMP-013; E10 §7 | — | — |
| TM-22 | AMP-18 | SRC-TURISMO | Axenda | 2026-11-09 | 19:30 | — | — | Conflito horario aberto | E4 EX01-COMP-011; E10 §5 | — | — |
| TM-23 | AMP-18 | SRC-LICEO | Programación do Liceo | 2026-11-09 | 16:30 | — | — | Prioridade provisional histórica, non hora canónica; coincide co cartel relatado | E8 V2; E10 §5 | — | 2026-11-02 |
| TM-24 | AMP-18 | — | Cartel relatado, emisor non precisado | 2026-11-09 | 16:30 | — | — | Outra superficie de evidencia relatada; non se conta como fonte adicional identificada | E4 EX01-COMP-011; E10 §5 | — | — |

## C. Solapamentos identificados

Contan só atribucións con `source_id` e estado Confirmada documentalmente. As publicacións adicionais conservan evidencia relatada: non hai nesta matriz un solapamento sustentado por contidos orixinais arquivados de ambas as fontes. As 12 atribucións primarias da Xunta son evidencia conservada, non proba de exclusividade.

| event_id | source_id coincidentes | Particularidade |
| --- | --- | --- |
| MUN-01 | SRC-CONCELLO; SRC-LAREGION | Relato previo; afirmacións temporais en B.2 cando corresponde. |
| MV-01 | SRC-MV; SRC-PRESSCLUB | Relato previo; afirmacións temporais en B.2 cando corresponde. |
| MV-02 | SRC-MV; SRC-TURISMO | Relato previo; afirmacións temporais en B.2 cando corresponde. |
| MV-03 | SRC-MV; SRC-PRESSCLUB; SRC-RADIOLIVERDADE | Relato previo; afirmacións temporais en B.2 cando corresponde. |
| MV-05 | SRC-MV; SRC-PRESSCLUB | Relato previo; afirmacións temporais en B.2 cando corresponde. |
| MV-07 | SRC-LAREGION; SRC-MV | Relato previo; afirmacións temporais en B.2 cando corresponde. |
| MV-08 | SRC-LAREGION; SRC-MV | Relato previo; afirmacións temporais en B.2 cando corresponde. |
| MV-09 | SRC-LAREGION; SRC-MV | Relato previo; afirmacións temporais en B.2 cando corresponde. |
| LR-03 | SRC-LAREGION; SRC-PRESSCLUB | Relato previo; afirmacións temporais en B.2 cando corresponde. |
| LR-04 | SRC-LAREGION; SRC-TURISMO | Relato previo; afirmacións temporais en B.2 cando corresponde. |
| LR-05 | SRC-LAREGION; SRC-LICEO; SRC-TURISMO | Relato previo; afirmacións temporais en B.2 cando corresponde. |
| AMP-09 | SRC-TEATRO; SRC-TURISMO | Comprobación anterior relatada; versións conservadas en B.2. |
| AMP-10 | SRC-TEATRO; SRC-TURISMO | Comprobación anterior relatada; versións conservadas en B.2. |
| AMP-18 | SRC-LICEO; SRC-TURISMO | Comprobación anterior relatada; versións conservadas en B.2. |

CatArte xa está compartido entre SRC-LAREGION e SRC-TURISMO, sen depender das dúas publicacións anónimas. «Non localizado na axenda consultada do centro» non xera unha relación negativa nin unha exclusividade. As restantes fontes para calquera evento quedan **sen información documental**, non ausentes.

## D. Lagoas e incidencias

| Caso | Información pendente / tratamento |
| --- | --- |
| MUN-01/02/03/06/07 | Cinco espazos individuais e fichas específicas sen transcribir. Non se asigna Auditorio polo seu carácter municipal. |
| 20 eventos MUN/MV/LR | Atribución principal identificada; falta o contido primario arquivado. A URL da ficha de Pateiro non equivale ao contido desa ficha. Non significa ausencia de contraste previo. |
| LR-04 | AT-44 e AT-45 conservan a web específica e a plataforma de venda sen fonte identificada. Precisar nome, URL e evidencia antes de asignar `source_id`. |
| MV-01 | TM-01–03:20:15/19:45 e posible aprazamento sen publicación nin data recuperadas. Non confirmar celebración nin eliminar o evento. |
| MV-02 | TM-04–05:04/11/10/11; EX01-COMP-010, sen selección canónica. |
| MV-03 | TM-06–08:19:45/19:30; EX01-COMP-004, conservar procedencia e consulta anterior de Radio. |
| MV-07 | TM-09–11: intervalos e superficies diferentes; EX01-COMP-001, sen intervalo canónico. |
| LR-05 | TM-12–14:20:00/19:30; EX01-COMP-005, non resolver por maioría. |
| 156460 e 157064 | EX01-XUNTA-001 e002: precisión xeográfica do teatro e punto de inicio do roteiro distinto do espazo asociado. Non se corrixen coordenadas nesta matriz. |
| LR-01 | A visita guiada de 05/11 segue pendente de clasificación; non se engade outra unidade. |
| Todos | Non hai exhaustividade das atribucións nin revisión suficiente para establecer exclusividades. As estatísticas de ICS de E9 non mapean novas relacións individuais dos 89. |

### Unidades compostas e sesións

Mantense o tratamento documental das sesións: os datos actuais poden conservarse nas notas, nas referencias e, só para conflitos, en B.2. O programa interno AMP-19/29 consérvase en E8 §Programación interna conservada e E10 §5, sen duplicar aquí as oito partes. Unha futura relación de compoñentes referenciaría o mesmo `event_id` e indicaría se é sesión ou parte, sen contala como evento adicional.

- MUN-03: unha programación de Samaín; relación completa de partes e horarios aínda pendente.
- MV-05: unha xornada; horario 09:00–14:15 relatado por Press Club e programa máis detallado, non varios eventos.
- LR-04: unha sesión de CatArte do 05/11, pertencente ao ciclo;12,19,26/11 fóra da xanela. Non sumar ademais o ciclo.
- LR-06: unha xornada con tres intervencións; non tres unidades.
- LR-07: só a sesión de Fina Casalderrey do 29/10, non o ciclo completo.
- MV-06 mantense separado de MV-05, malia compartir centro e data. As exposicións prolongadas seguen como unha unidade cada unha.

- AMP-25: 06/11 ás 19:00 e 07/11 ás 17:30, unha actividade; PV-01: 29/30 outubro; PV-04: 30/31 outubro e 06/07 novembro, unha unidade cada unha.
- AMP-19: ciclo composto, 05/11 de 13:00–21:00; tres sesións/intervencións en E8, non tres eventos. AMP-29: programa do 07 e 11/11, non actividade continua entre datas.
- MUS-01 e MUS-14: dúas actuacións de jazz segundo a decisión recibida; MUS-19, MUS-22 e AMP-28 non se desagregan. AMP-26 conserva só a convocatoria 05/11; a de 19/11 queda fóra.

### Lagoas específicas da ampliación

- AMP-01/03/04: faltan intervalo e espazo, ademais da fonte publicadora. AMP-02 conserva Marisa Marimón como sede, non como publicadora; falta recuperar a versión alternativa do fin.
- AMP-08: sede individual e publicación específica pendentes. AMP-11–13: sedes e horas descoñecidas, malia a fonte MAPOU identificada.
- MUS: só V2 permite confirmar documentalmente a atribución ao Liceo de MUS-15/21/23. MUS-02 non se atribúe ao Liceo pola sede. O resto require recuperar publicacións, non supoñer unha fonte por local.
- Cineclube: asociación dos tres filmes ao cineclube e canle de programación identificadas, pero as fichas individuais non se leron na comprobación anterior. Mantéñense tres atribucións **probables**, sen entrar no reconto de solapamentos confirmados. Radio si ten publicacións de AMP-06/07 expresamente relatadas en V1.
- AMP-14/25: carteis mencionados, emisor sen identificar. AMP-23/24: a mención xenérica de carteis de Forasteiro non permite asignar unha publicación concreta a cada convocatoria; quedan sen relación, non se extrapola Instagram de FOR-03. As dúas atribucións de carteis AMP-14/25 quedan pendentes.
- AMP-16/17/20/21/22/26/27: datos relatados non identifican suficientemente o publicador. Nobel, Torgal, Pita, Riquiño, Biblioteca Nós e Ponte Vella como sedes non acreditan por si sós fontes.
- AMP-09/18: discrepancias horarias abertas; AMP-10: incompletitude de funcións. E10 priorizaba provisionalmente o cartel de Recunchos; consérvase esa decisión histórica sen converter 16:30 en hora canónica.
- Patakana, ópera e conferencia climática seguen non incorporadas; Freaks segue excluída do período e coa discrepancia en E4 EX01-COMP-014. Non se crean filas adicionais nin se eliminan incluídos por falta de orixinais.

## E. Avaliación metodolóxica

O modelo permite representar os 89 eventos e as lagoas sen crear fontes a partir de sedes. Non se precisan táboas adicionais de arquitectura. As 57 filas novas non equivalen a 57 atribucións: algunhas teñen varias, outras só indicios, publicacións anónimas ou ningunha fonte identificada.

| Métrica | Viabilidade actual | Interpretación |
| --- | --- | --- |
| Eventos documentados por fonte | Calculable parcialmente | Reconto reproducible das atribucións confirmadas desta matriz; non todos os anuncios da fonte. Probables separados. |
| Eventos compartidos | Calculable parcialmente | Coincidencias documentais positivas; non total exhaustivo de publicacións compartidas. |
| Solapamentos por pares | Calculable parcialmente | Pares positivos da táboa C; cero documental non acredita ausencia real. |
| Porcentaxe dos 89 atribuída a cada fonte | Calculable como mínimo documental | Reconto confirmado / 89; non cobertura exhaustiva nin estimación da oferta cultural total. |
| Exclusividades | Non calculable | Unha soa fonte documentada non proba exclusividade; non hai relacións negativas verificadas. |
| Eventos sen fonte confirmada | Calculable documentalmente | Déficit da matriz, non eventos sen publicación real. |
| Celebración efectiva / integridade global | Non calculable | Un anuncio e unha comprobación relatada non acreditan celebración nin exhaustividade. |

O seguinte paso útil é recuperar a identidade do publicador e a referencia de publicación dos eventos sen atribución confirmada, comezando polas actuacións MUS e polos carteis anónimos. Non é imprescindible cambiar o modelo para esa revisión.

## F. Validación e resumo cuantitativo

| Medida | Resultado | Definición |
| --- | --- | --- |
| Eventos distintos | 89 | 32 orixinais + 23 MUS + 29 AMP + 4 PV + 1 FOR |
| Fontes identificadas | 16 | 8 anteriores + 8 novas; Cineclube só con atribucións probables |
| Atribucións totais | 77 | 47 orixinais + 30 novas; IDs continuos |
| Atribucións confirmadas documentalmente | 70 | Con source_id; non implica celebración |
| Atribucións probables | 3 | Tres filmes asociados ao Cineclube, sen publicación individual acreditada |
| Atribucións pendentes | 4 | Dúas de CatArte + dúas de carteis na ampliación |
| Contido primario conservado | 12 | 12 payloads Xunta, sen incremento |
| Comprobacións anteriores relatadas | 62 | Inclúe pendentes de identificación; non son orixinais |
| Indicios documentados | 3 | Só atribucións probables Cineclube |
| Eventos con varias fontes confirmadas | 14 | Só fontes identificadas e estado confirmado |
| Eventos cunha soa fonte confirmada | 40 | Non exclusivos; AMP-06/07 teñen ademais indicio Cineclube |
| Eventos sen fonte confirmada | 35 | Inclúe AMP-08 cunha fonte probable |
| Eventos sen ningún source_id, nin probable | 34 | Descoñecido non equivale a ausencia real |
| Afirmacións temporais | 24 | TM-01–14 intactas + 10 novas |
| Eventos con conflitos temporais | 8 | 5 do piloto + AMP-02/09/18; AMP-10 é incompletitude de funcións, non noveno conflito |
| Eventos en B.2 | 9 | 8 conflitos + 1 con información parcial de funcións |

**Eventos sen atribución confirmada:** MUS-01, MUS-02, MUS-03, MUS-04, MUS-05, MUS-06, MUS-07, MUS-08, MUS-09, MUS-10, MUS-11, MUS-12, MUS-13, MUS-14, MUS-16, MUS-17, MUS-18, MUS-19, MUS-20, MUS-22, AMP-01, AMP-03, AMP-04, AMP-08, AMP-14, AMP-16, AMP-17, AMP-20, AMP-21, AMP-22, AMP-23, AMP-24, AMP-25, AMP-26, AMP-27.

**Regra de reprodución:** contar IDs únicos de A; en B contar AT únicos por estado/tipo de evidencia. Para cada evento, contar source_id distintos só nas filas Confirmada documentalmente. Os pendentes sen source_id e as probables non entran nos solapamentos positivos. Un mesmo evento con tres fontes produce tres pares, non tres eventos compartidos.

### Atribucións por fonte

Non é cobertura exhaustiva. A suma de atribucións confirmadas é 70, non 70 eventos distintos; hai 54 eventos con algunha fonte confirmada.

| source_id | Eventos con atribución confirmada | Eventos con atribución probable | Mínimo documental confirmado / 89 |
| --- | --- | --- | --- |
| SRC-CHINITA-IG | 1 | 0 | 1/89 (1.1 %) |
| SRC-CINECLUBE | 0 | 3 | 0/89 (0.0 %) |
| SRC-CONCELLO | 6 | 0 | 6/89 (6.7 %) |
| SRC-FORASTEIRO-IG | 1 | 0 | 1/89 (1.1 %) |
| SRC-FRRII | 1 | 0 | 1/89 (1.1 %) |
| SRC-LAREGION | 11 | 0 | 11/89 (12.4 %) |
| SRC-LICEO | 6 | 0 | 6/89 (6.7 %) |
| SRC-MAPOU | 3 | 0 | 3/89 (3.4 %) |
| SRC-MV | 8 | 0 | 8/89 (9.0 %) |
| SRC-PONTEVELLA | 4 | 0 | 4/89 (4.5 %) |
| SRC-PRESSCLUB | 4 | 0 | 4/89 (4.5 %) |
| SRC-RADIOLIVERDADE | 3 | 0 | 3/89 (3.4 %) |
| SRC-TEATRO | 2 | 0 | 2/89 (2.2 %) |
| SRC-TURISMO | 7 | 0 | 7/89 (7.9 %) |
| SRC-UVIGO | 1 | 0 | 1/89 (1.1 %) |
| SRC-XUNTA | 12 | 0 | 12/89 (13.5 %) |

### Solapamentos positivos por pares

Só coincidencias confirmadas documentalmente. Non se crean filas de cero para os pares sen evidencia.

| Fonte A | Fonte B | Eventos | Identificadores |
| --- | --- | --- | --- |
| SRC-CONCELLO | SRC-LAREGION | 1 | MUN-01 |
| SRC-LAREGION | SRC-LICEO | 1 | LR-05 |
| SRC-LAREGION | SRC-MV | 3 | MV-07, MV-08, MV-09 |
| SRC-LAREGION | SRC-PRESSCLUB | 1 | LR-03 |
| SRC-LAREGION | SRC-TURISMO | 2 | LR-04, LR-05 |
| SRC-LICEO | SRC-TURISMO | 2 | LR-05, AMP-18 |
| SRC-MV | SRC-PRESSCLUB | 3 | MV-01, MV-03, MV-05 |
| SRC-MV | SRC-RADIOLIVERDADE | 1 | MV-03 |
| SRC-MV | SRC-TURISMO | 1 | MV-02 |
| SRC-PRESSCLUB | SRC-RADIOLIVERDADE | 1 | MV-03 |
| SRC-TEATRO | SRC-TURISMO | 2 | AMP-09, AMP-10 |

### Integridade e límites da revisión

- 89 IDs únicos e correspondencia exacta cos 32 anteriores máis as 57 filas consolidadas E8; sen altas de eventos nin cambios de agrupación.
- AT-01–47 e TM-01–14 consérvanse literalmente, incluídas AT-44/45 de CatArte. Ningunha atribución nova cambia os 32 iniciais.
- Os oito source_id anteriores consérvanse. Todas as atribucións identificadas apuntan ao catálogo e as novas teñen referencia documental; as parellas evento–fonte identificada non se repiten.
- As filas anónimas non se deduplican entre si como unha suposta fonte única. Identificalas podería requirir reconciliar atribucións, sen crear máis eventos.
- As ligazóns relativas de referencias tiñan sintaxe Markdown normal no ficheiro. Non se atopou o erro literal `\(` nesas ligazóns; non se cambian os destinos.
- Esta validación comproba consistencia documental, non a verdade de cada anuncio. As cifras históricas de incorporación Xunta12/MUN5/MV8/LR7 non son a cobertura final das fontes.

## Estado de Git e entrega

Só se amplía este documento de traballo na rama `docs/experiment-01-classification`. Segue sen seguimento no índice; inventarios e evidencias consolidados intactos. Non se fai commit, push nin PR. Detense a ampliación para revisión.
