# OBJETIVO SMART Y ANÁLISIS DE VIABILIDAD

**Asignatura:** Gestión de Proyectos de Software (SCG-1009)

**Unidad:** 3. Planificación del proyecto

**Proyecto:** Plataforma para artesanas textiles de la Región Mixteca

**Lugar:** Región Mixteca, Oaxaca

**Metodología:** eduScrum

**Equipo de desarrollo:** Mari Cruz Gomez, Carla Bautista León, Alan Sahid Cortes, Aldair Gonzalez

---

## 1. Formulación del objetivo SMART

### Objetivo del proyecto

Desarrollar y validar Open Hub Tec, una plataforma de software con blockchain que ayude a las artesanas y talleres textiles de la Región Mixteca de Oaxaca con tres problemas que identificamos: el plagio de sus diseños, el intermediarismo que les quita control sobre el precio de sus piezas y la falta de canales para venderlas. La plataforma permitirá registrar la autoría de diseños con hash y timestamp, generar reportes verificables, registrar ventas con su tiempo de elaboración, consultar historiales de precios, publicar perfiles verificados de taller y llevar el control de pedidos y anticipos. Blockchain se usa solo donde sirve para algo concreto: integridad, trazabilidad y evidencia verificable. El sistema debe poder usarse desde el celular y tomar en cuenta la conectividad limitada de la región. El trabajo se hará con eduScrum de agosto a diciembre de 2026 y se verificará con las seis historias de usuario auditadas en el Sprint 1 (HU-1.1, HU-1.2, HU-2.1, HU-2.2, HU-3.1 y HU-3.2), con criterios de aceptación y pruebas funcionales. Además, se evaluará si el proyecto puede sostenerse con financiamiento Web3 (Stellar Community Fund y Drips Protocol).

### Desglose de las dimensiones SMART

**S – Específico:** construir una plataforma que registre diseños textiles con hash y fecha, genere reportes de verificación de autoría, guarde ventas con tiempo de elaboración y precio, muestre historiales de precios, publique perfiles verificados y gestione pedidos y anticipos para artesanas de la Mixteca.

**M – Medible:** cumplir el 100 % de los criterios de aceptación de las historias seleccionadas; que el sistema rechace registros con datos obligatorios faltantes (por ejemplo, una venta sin tiempo de elaboración); que ningún registro confirmado se pueda modificar; y que no quede ningún error crítico conocido al terminar las pruebas. En lo financiero, la meta es dejar un dictamen Go / No-Go basado en el costo de calidad calculado en el Sprint 2 (34 h, $3,400 MXN) contrastado contra las fuentes de financiamiento Web3.

**A – Alcanzable:** el trabajo se divide en incrementos con eduScrum y se prioriza el backlog (cinco historias con prioridad Alta y una Media). Las historias ya pasaron por una auditoría con IA que quitó ambigüedades y dejó un alcance acotado, y se usan herramientas gratuitas y redes de prueba, así que el costo en efectivo es bajo. Las 142 horas estimadas se reparten entre cuatro integrantes, unas 35 h por persona a lo largo del periodo.

**R – Relevante:** responde a necesidades documentadas de tejedoras de la Mixteca: demostrar que un diseño es suyo si alguien lo copia, conocer y registrar lo que realmente cobran por sus piezas, y ganar visibilidad sin depender solo de intermediarios o ferias ocasionales.

**T – Temporalizado:** planificación, desarrollo, pruebas y documentación entre agosto y diciembre de 2026. Las fechas de entrega de cada Sprint se registran en el tablero eduScrum.

---

## 2. Trazabilidad con los Sprints 1 y 2

Este documento no parte de cero: se apoya en lo que ya se hizo en los dos primeros sprints.

| Sprint | Artefacto | Cómo se usa en este documento |
|---|---|---|
| Sprint 1 | Historias de usuario auditadas (HU-1.1 a HU-3.2), con criterios de aceptación y backlog priorizado | Definen el alcance del objetivo SMART, la métrica de cumplimiento y los requisitos técnicos de la sección 3. |
| Sprint 2 | Plan de calidad y Costo de la Calidad (CoQ) | Son la base de las estimaciones de horas y costos de la sección 4. |

### A. Relación con las historias de usuario auditadas (Sprint 1)

| ID | Problemática | Historia | Corrección de la auditoría y qué debe cumplir |
|---|---|---|---|
| HU-1.1 | Plagio y apropiación cultural | Registro de autoría de un diseño textil | Se definió el uso de hash, timestamp y bloqueo de modificaciones; las correcciones solo como versión nueva enlazada; aval comunitario obligatorio en autoría colectiva. |
| HU-1.2 | Plagio y apropiación cultural | Verificación pública de autoría ante disputa | Se limitó la información pública para proteger datos sensibles; reporte verificable sin cuenta que muestra qué registro es anterior. |
| HU-2.1 | Intermediarismo y precio injusto | Registro de venta directa de una pieza | Se volvió obligatorio el tiempo de elaboración; guardado local sin internet y sincronización posterior; promedio de 12 meses por prenda. |
| HU-2.2 | Intermediarismo y precio injusto | Consulta de precio e historial de ventas | Se quitó "precio justo": el sistema solo muestra precios y tiempos con registros confirmados; "Información privada" si el historial no es público. |
| HU-3.1 | Falta de comercialización | Perfil verificado de taller artesanal | Se quitó el "nivel de confianza" subjetivo: solo ventas confirmadas y fecha de creación del perfil. |
| HU-3.2 | Falta de comercialización | Gestión de pedidos y apartados | Si se cancela un pedido con anticipo, se conserva el registro original y se agrega el estado "Cancelado — pendiente de reembolso". |

### B. Costo de la calidad (Sprint 2)

El CoQ nos dice cuánto esfuerzo se va en prevenir errores, revisar que todo funcione y corregir lo que falle. Las horas son estimaciones académicas y se valoran con un costo de referencia de **$100 MXN por hora**.

| Categoría de CoQ | Actividades en Open Hub Tec | Horas | Costo (MXN) |
|---|---|---|---|
| Prevención | Revisar historias y criterios; definir datos obligatorios; decidir qué va dentro y fuera de la cadena; validaciones de fechas, montos y tallas; diseñar pruebas antes de programar; analizar riesgos de conectividad. | 12 h | $1,200 |
| Evaluación | Probar hash y timestamp; probar que los registros no se editen; rechazo de ventas sin tiempo de elaboración; modo sin conexión y sincronización; cálculo de promedios; estados y notificaciones de pedidos; usabilidad en celular. | 10 h | $1,000 |
| Fallas internas | Corregir cálculos y validaciones, duplicados y registros editables, y repetir pruebas. | 8 h | $800 |
| Fallas externas | Atender reportes de artesanas o compradores, corregir información mal mostrada, recuperar registros perdidos, corregir datos personales expuestos por error. | 4 h | $400 |
| **Total CoQ** | Suma de las cuatro categorías | **34 h** | **$3,400** |

Desglose rápido: prevención y evaluación (costos de buena calidad) suman 22 h y $2,200; fallas internas y externas (costos de mala calidad) suman 12 h y $1,200.

Estos montos son estimaciones académicas, no gastos reales. Se van ajustando con las horas reales, las pruebas hechas y los defectos registrados.

---

## 3. Análisis de viabilidad técnica y operativa

### A. Viabilidad técnica

- **Gestión de la información y uso de blockchain:** hay que guardar diseños, fechas, técnicas, comunidades, ventas, precios, tiempos de elaboración, perfiles y pedidos. Lo que se escribe en blockchain no se puede borrar, así que las fotos y datos personales no deberían ir directamente en la cadena; lo que va a la cadena es el hash y la marca de tiempo, y el resto se guarda fuera.
- **Integridad de los datos:** el sistema debe impedir campos obligatorios vacíos, fechas inválidas y montos inconsistentes, y no permitir modificar registros originales; las correcciones se guardan como registros nuevos enlazados.
- **Privacidad:** los reportes y perfiles públicos no muestran datos personales sensibles sin autorización, y cada historial respeta si la tejedora lo marcó como público o privado.
- **Conectividad limitada:** en varias comunidades de la Mixteca la señal es intermitente o no existe. La HU-2.1 exige guardar la venta en el teléfono sin internet y sincronizarla después. Esto implica guardar localmente, evitar duplicados al sincronizar y confirmar el registro en blockchain cuando regrese la señal. Es el reto técnico más importante del proyecto.
- **Dispositivos y usabilidad móvil:** la mayoría de las usuarias van a usar el celular, probablemente de gama básica y con poco almacenamiento. Los formularios deben ser simples, con pocas fotos pesadas y sin pasos innecesarios.
- **Infraestructura blockchain:** el desarrollo y las pruebas se hacen en redes de prueba (testnet) y con herramientas gratuitas o de código abierto. Pasar a una red real implicaría revisar comisiones de transacción y el manejo de claves de las usuarias.
- **Notificaciones:** la HU-3.2 pide notificaciones automáticas al comprador; hay que definir por qué medio se envían, considerando que puede no haber internet constante.
- **Cálculos:** el cálculo del promedio de 12 meses se prueba con datos conocidos y solo con registros confirmados.

**Evaluación técnica:** viable con condiciones. Los requisitos están definidos y son verificables, pero la decisión sobre qué guardar en cadena y la solución del modo sin conexión deben validarse con un prototipo temprano.

### B. Viabilidad operativa mediante eduScrum

- **Autogestión:** el equipo trabaja con tablero eduScrum (pendiente, en proceso, terminado), responsables, prioridades y evidencias, y se organiza solo bajo la supervisión del eduScrum Master, que ayuda a quitar impedimentos y cuida que se sigan los acuerdos.
- **Organización y backlog:** análisis, diseño, programación, pruebas y documentación se reparten con responsables y fechas. Las dependencias del backlog importan: la HU-1.2 necesita la HU-1.1, y la HU-2.2 necesita los registros de la HU-2.1.
- **Restricciones del aula:** el proyecto se hace dentro de un periodo escolar, con horas de clase limitadas, otras materias que compiten por el tiempo, equipos personales y el internet de la institución. Seis historias con blockchain es mucho para un solo periodo, por eso se prioriza.
- **Restricciones del contexto:** para validar con las artesanas hay que coordinar visitas o contacto remoto con una región que tiene distancias largas y conectividad irregular, así que la retroalimentación puede llegar más lenta.
- **Revisión y retroalimentación:** al final de cada Sprint se revisan criterios de aceptación y resultados de pruebas, y se hace una retrospectiva para ajustar el siguiente.

**Evaluación operativa:** viable con condiciones. Depende de mantener el backlog actualizado, repartir bien las tareas y reducir el alcance si el tiempo no alcanza.

---

## 4. Viabilidad financiera Web3 y dictamen Go / No-Go

### A. Estructura de costos

Se usa un costo académico de referencia de **$100 MXN por hora de trabajo**. Son estimaciones, no gastos reales.

| Concepto | Descripción | Horas | Costo (MXN) |
|---|---|---|---|
| Análisis y diseño | Revisión de requisitos, historias y diseño de la solución | 16 h | $1,600 |
| Desarrollo | Programación de las seis historias, incluida la parte blockchain | 80 h | $8,000 |
| Calidad (CoQ) | Prevención, evaluación y corrección según el Sprint 2 | 34 h | $3,400 |
| Documentación y capacitación | Manuales y orientación a las artesanas | 12 h | $1,200 |
| Infraestructura | Alojamiento, almacenamiento de fotos y servicios; se usan planes gratuitos durante el curso | 0 h | $0 |
| Comisiones de red | Transacciones en blockchain; en testnet no tienen costo real | 0 h | $0 en pruebas (por estimar en producción) |
| **Costo total** | Suma de los costos aplicables | **142 h** | **$14,200** |

El costo de calidad ($3,400) es solo una parte del total; el desarrollo es lo que más pesa ($8,000, cerca del 56 %). Además, todo el costo del curso es trabajo del equipo, así que el **gasto en efectivo durante el periodo es de $0**.

### B. Fuentes de financiamiento Web3

**Stellar Community Fund (SCF).** Según el SCF Handbook, son premios de entre $10,000 y $100,000 USD pagados en XLM, que se deciden por votación de la comunidad y se dirigen a proyectos construidos sobre Stellar y Soroban. Las rondas de Build Award se abren cada seis semanas y también existe un camino de entrada llamado Kickstart. Es financiamiento por hitos, no continuo, y no está asegurado: hay que postular, presentar un proyecto que use Stellar de forma real y ganar la votación. Los montos y requisitos hay que confirmarlos en la convocatoria vigente.

**Drips Protocol.** Drips permite enviar fondos en flujos continuos con liquidación por segundo, además de donaciones únicas, y se pueden armar listas (Drip Lists) para repartir fondos entre varios destinatarios. Su valor para nosotros es el financiamiento continuo, que sirve para mantener la plataforma después de un premio único, o para repartir ingresos entre colaboradoras. La documentación revisada describe a Drips como un protocolo para cadenas EVM, así que hay que confirmar cómo se integra con una solución en Stellar antes de contar con él en el plan.

| Fuente | Tipo | Qué podría cubrir | Estado |
|---|---|---|---|
| SCF (Kickstart / Build Award) | Premio por hitos, en XLM, por votación | Desarrollo, infraestructura y comisiones de la etapa de producción | Por postular; no confirmado |
| Drips Protocol | Flujo continuo de fondos | Mantenimiento recurrente y reparto entre colaboradoras | Por validar integración; no confirmado |
| Recursos propios e institución | Horas del equipo, equipos y laboratorios | Costo académico de desarrollo y calidad ($14,200 MXN en horas) | Disponible durante el periodo |
| Herramientas gratuitas y testnet | Costo cero | Desarrollo y pruebas | Disponible |

### C. Contraste costo vs. financiamiento

| Concepto | Monto |
|---|---|
| Costo total estimado del proyecto (horas del equipo) | $14,200 MXN (142 h) |
| Costo de calidad (CoQ) | $3,400 MXN (34 h) |
| Gasto en efectivo durante el curso | $0 MXN |
| Premio SCF (rango del handbook) | $10,000 a $100,000 USD en XLM |

Durante el periodo académico el costo real en efectivo es nulo, porque el trabajo son horas del equipo, se usan herramientas gratuitas y las pruebas son en testnet. Por eso el proyecto no depende de ganar un fondo para llegar a diciembre. El financiamiento Web3 se necesita para la segunda etapa: salir a producción con comisiones reales, almacenamiento, soporte y capacitación a las artesanas. Incluso el premio más bajo del SCF (USD $10,000) está muy por encima del costo total de $14,200 MXN, más de diez veces, así que cubriría con holgura la etapa de producción, mientras que Drips ayudaría a dar continuidad. El riesgo es que ninguna de las dos fuentes está asegurada, así que el plan no debe depender de ellas para el cierre del curso.

### D. Dictamen Go / No-Go

| Dimensión | Dictamen | Justificación |
|---|---|---|
| Técnica | GO condicionado | Requisitos definidos y verificables; falta validar con un prototipo el registro sin conexión y la separación de datos dentro y fuera de la cadena. |
| Operativa | GO condicionado | Backlog priorizado, tablero y roles definidos; el riesgo es el tiempo del periodo para seis historias (142 h entre cuatro integrantes). |
| Financiera | GO | Gasto en efectivo de $0 durante el curso y costo total de $14,200 MXN en horas; SCF y Drips son oportunidades para la etapa de producción, no requisitos para terminar. |

**Dictamen final: GO condicionado.** Se decide continuar con el proyecto, con estas condiciones: (1) validar el modo sin conexión con un prototipo antes de la mitad del periodo; (2) ajustar las estimaciones de horas y costos con las horas reales que se vayan registrando; (3) arrancar con las historias de prioridad Alta y dejar la HU-2.2 para después si el tiempo aprieta; (4) confirmar los requisitos del SCF y la compatibilidad de Drips antes de incluirlos en el plan de sostenibilidad.

**Criterios de NO-GO:** el dictamen cambia si el registro sin conexión resulta inviable con las herramientas disponibles, si el equipo no logra completar al menos las historias prioritarias en el periodo, o si los costos reales rebasan los recursos disponibles sin una alternativa de financiamiento. En ese caso se reduciría el alcance a una sola problemática o se pausaría el proyecto.

---

## 5. Gestión del equipo y gobernanza eduScrum

### A. Organización del equipo

- **eduScrum Master:** [Nombre]. Cuida que se siga el marco eduScrum, ayuda a quitar impedimentos y supervisa sin decidir por el equipo.
- **Product Owner:** [Nombre]. Valida prioridades y requisitos.
- **Equipo de desarrollo:** Mari Cruz Gomez, Carla Bautista León, Alan Sahid Cortes y Aldair Gonzalez. Se encargan del análisis de requisitos, el desarrollo (incluida la parte blockchain), las pruebas de calidad y la documentación, registrados por nombre en el tablero.

### B. Autogestión, seguimiento y control

- Tablero eduScrum con tareas, responsables, prioridades, estados y evidencias.
- Reuniones breves de seguimiento para ver avances e impedimentos.
- Revisión y retrospectiva al final de cada Sprint para ajustar el trabajo.
- Registro de horas de prevención, evaluación y corrección para actualizar el CoQ.
- Registro de errores encontrados y acciones para resolverlos.
- Capturas, resultados de pruebas y demás evidencias guardadas.
- GitHub para el historial de cambios y la coordinación de la documentación.

### C. Criterios de finalización

Una historia se considera terminada cuando cumple sus criterios de aceptación, pasó las pruebas, no tiene defectos críticos conocidos, tiene evidencias de las pruebas, cuenta con la documentación necesaria y fue revisada conforme a la Definición de Hecho (DoD) que acordó el equipo.

---

## 6. Conclusión

Open Hub Tec busca ayudar a las artesanas textiles de la Mixteca con el plagio de sus diseños, el intermediarismo y la falta de canales de venta, usando blockchain solo donde aporta integridad, trazabilidad y evidencia verificable. El objetivo SMART deja claro qué se va a hacer, cómo se mide y en qué tiempo, y la trazabilidad con los Sprints 1 y 2 conecta el alcance con las historias auditadas y los datos de calidad (34 h y $3,400 MXN de CoQ).

En lo técnico, lo más delicado es el registro sin conexión y decidir qué datos van dentro de la cadena. En lo operativo, eduScrum nos permite organizarnos, pero el tiempo del periodo obliga a priorizar. En lo financiero, el costo total estimado es de $14,200 MXN en horas de trabajo, sin gasto en efectivo durante el curso, y Stellar Community Fund y Drips Protocol son oportunidades para sostener el proyecto después, no algo asegurado.

Por todo eso, el dictamen es GO condicionado: el proyecto se puede hacer, siempre que se cumplan las condiciones de la sección 4 y se ajusten las estimaciones con las horas reales del equipo.
