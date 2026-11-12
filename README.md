# charly-vibes

Se dice por ahí que el software es una disciplina de lógica pura. Uno se sienta, tipea, y el universo obedece. Qué mentira más elegante.

Esto, entonces, no es una persona. "Charly Vibes" es más bien un campo de pruebas, una zona de desastre controlada. Un intento de registrar el pulso de una nueva forma de delirio: el código asistido por una inteligencia que no es ni inteligente ni artificial, sino algo intermedio y mucho más extraño. Algunos lo llaman *vibe coding*. Acá se busca algo más parecido a una [resonancia](https://charly-vibes.github.io/microdancing/es/posts/resonant-coding.html): encontrar la frecuencia correcta para que el caos se ordene, como esas ondas estacionarias que aparecen cuando uno agita una soga con precisión.

Cada línea aquí es producto de ese diálogo febril, una conversación con un oráculo que cobra por palabra. El trabajo ya no se mide en horas-silla, sino en tokens quemados, en un contador que avanza como un taxímetro hacia la bancarrota existencial. Uno paga por pensar, o por hacer que algo piense por uno. La diferencia es cada vez más borrosa. Mientras haya plata para los tokens, se sigue trabajando. Cuando se acabe, habrá que ver qué otro delirio inventamos.

El objetivo, si es que hay uno, es descular qué forma tomará este oficio. Hay una obsesión por la planificación, por revisar las respuestas de la máquina como quien lee las entrañas de un pollo de silicio.

## Las exploraciones

### El ecosistema

Los CLIs y la infraestructura compartida que sostienen todo: capturar el contexto, verificar el comportamiento, seleccionar los tests, analizar el código. Casi todos en Rust, más un orfebre en Go. Varios siguen en etapa de especificación, y así se dice en cada ficha.

*   **[wai](https://charly-vibes.github.io/wai/)** · [repo](https://github.com/charly-vibes/wai): Gestor de flujos de trabajo para desarrollo asistido por IA. Organiza los artefactos de un proyecto —investigación, planes, diseños— capturando el *por qué* detrás de cada decisión. El cuaderno de bitácora que la máquina necesita para no perderse.
*   **[fabbro](https://charly-vibes.github.io/fabbro/)** · [repo](https://github.com/charly-vibes/fabbro): Una herramienta de orfebre digital. Un martillo y cincel para la línea de comandos, para revisar y comentar lo que nos vomitan los modelos de lenguaje. Anotaciones estructuradas sobre código, local-first, sin servidores.
*   **[dont](https://charly-vibes.github.io/dont/)** · [repo](https://github.com/charly-vibes/dont): CLI para obligar a agentes autónomos a fundamentar sus afirmaciones antes de hacerlas. Primero el grounding, después el verbo.
*   **[specodelic](https://charly-vibes.github.io/specodelic/)** · [repo](https://github.com/charly-vibes/specodelic): Formato de especificaciones en Markdown —un archivo da Intent, Constraints, Model y Properties— y CLI (`spk`) que lo lintea, compila, verifica y refactorea. Para que un spec pueda fallar en CI en lugar de subdeterminar la build en silencio.
*   **[espectacular](https://charly-vibes.github.io/espectacular/)** · [repo](https://github.com/charly-vibes/espectacular): Capa de verificación de comportamiento para el ecosistema de desarrollo IA de charly. Una herramienta para asegurar que los agentes se mantengan dentro de los límites esperados.
*   **[testaruda](https://charly-vibes.github.io/testaruda/)** · [repo](https://github.com/charly-vibes/testaruda): Motor de selección de tests con semiring de procedencia. Dado un cambio de código, computa el conjunto de tests afectados mediante análisis incremental de dependencias.
*   **[pretender](https://charly-vibes.github.io/pretender/)** · [repo](https://github.com/charly-vibes/pretender): Herramienta de análisis de código basada en tree-sitter que genera reportes SARIF. Una pieza más del rompecabezas de calidad de código asistida.
*   **[vampiro](https://charly-vibes.github.io/vampiro/)** · [repo](https://github.com/charly-vibes/vampiro): CLI en Rust que verifica si el código compone correctamente a través de límites de llamada, módulo, efecto, ley, retry, recurso y confianza. En cada borde: ¿este edge compone válidamente en la categoría que dice componer?
*   **[wild](https://charly-vibes.github.io/wild/)** · [repo](https://github.com/charly-vibes/wild): Compatibilidad y composición de componentes verificadas por máquina, modeladas como una categoría de contratos. `wild extract` y `wild check` ya están implementados y testeados en runtime.
*   **[crua](https://charly-vibes.github.io/crua/)** · [repo](https://github.com/charly-vibes/crua): CLI en Rust, en etapa de especificación, que verifica si el código respeta el modelo de costo del hardware y runtime donde se ejecuta: layout de cache lines, estabilidad de tipos, modelos de concurrencia, contención de locks.
*   **[livin](https://charly-vibes.github.io/livin/)** · [repo](https://github.com/charly-vibes/livin): CLI en Rust, en etapa de especificación, que comprueba si una suite de tests realmente ejercita los valores borde que la forma del propio código implica: cero, vacío, singleton, duplicado, overflow, cada rama de un sum type.
*   **[sunset](https://github.com/charly-vibes/sunset)** · [repo](https://github.com/charly-vibes/sunset): Extracción local de documentos: PDF a texto buscable con referencias verificables a la fuente. Su formato DSC retiene ubicaciones, productores, transformaciones y omisiones, para que cada pasaje se pueda cotejar contra la página original.
*   **[bajan](https://charly-vibes.github.io/bajan/)** · [repo](https://github.com/charly-vibes/bajan): Pipeline CLI de grafos de conocimiento guiado por specs: ingesta de fuentes, extracción de claims, consulta del grafo. Rust con triple store en SQLite y la procedencia como estructura del grafo.
*   **[whisper](https://charly-vibes.github.io/whisper/)** · [repo](https://github.com/charly-vibes/whisper): CLI en Rust que hace determinista el skill `whisper` de incitaciones. Rutas canónicas de repos, entradas de conocimiento idempotentes y serving de contexto con presupuesto: la capa mecánica convertida en binario. El comando es `turu`.
*   **[fck](https://github.com/charly-vibes/fck)** · [repo](https://github.com/charly-vibes/fck): Kit de cuatro skills para agentes de código: diagnóstico sin rodeos cuando la frustración apunta a la máquina. Una lectura de Le Guin aplicada a cómo le hablamos a la IA.
*   **[funkalization](https://charly-vibes.github.io/funkalization/)** · [repo](https://github.com/charly-vibes/funkalization): Espacio de trabajo semántico para diseño de software: propone, revisa e inspecciona diseños preservando significado, autoridad y evidencia. Propuestas tipeadas, decisiones con guardas, evidencia acotada.
*   **[gently](https://charly-vibes.github.io/gently/)** · [repo](https://github.com/charly-vibes/gently): Port a Rust del Graph::Easy de Perl: parsea, distribuye y renderiza grafos como ASCII art, boxart, HTML o DOT. "Everything is connected".
*   **[genesis](https://charly-vibes.github.io/genesis/)** · [repo](https://github.com/charly-vibes/genesis): Crate de Rust compartida con la infraestructura transversal del suite: sobres de JSON, CLI, self-healing. El fundamento común que el rompecabezas necesitaba.
*   **[evallerina](https://github.com/charly-vibes/evallerina)** · [repo](https://github.com/charly-vibes/evallerina): Evals con avatar: batería de evaluación para la familia dulce-de-leche. Mide empíricamente si los agentes LLM leen, parsean y actúan sobre los canales de salida AIX del suite: sobres JSON, sugerencias de self-healing, bloques administrados.
*   **[dulce-de-leche](https://charly-vibes.github.io/dulce-de-leche/)** · [repo](https://github.com/charly-vibes/dulce-de-leche): Un comando para instalar, configurar y actualizar todas las herramientas de charly-vibes. El repo queda limpio: todo vive bajo `.ddl/`.

### La palabra

Lo que se escribe mientras se construye: la bitácora, el método, la receta y el ritual. Si el código es efímero, esto intenta quedarse.

*   **[microdancing](https://charly-vibes.github.io/microdancing/)** · [repo](https://github.com/charly-vibes/microdancing): Microposts. Apuntes al margen. Crónicas de lo mínimo, ideas fugaces atrapadas antes de que se disuelvan. Ahí vive el manifiesto del [Resonant Coding](https://charly-vibes.github.io/microdancing/es/posts/resonant-coding.html) y su [guía práctica](https://charly-vibes.github.io/microdancing/es/posts/resonant-coding-guia.html).
*   **[rizomas](https://charly-vibes.github.io/rizomas/)** · [repo](https://github.com/charly-vibes/rizomas): Explicaciones rizomáticas. Un experimento en gestación, una raíz que busca tierra donde crecer. Todavía no se sabe qué forma va a tomar, y eso está bien.
*   **[incitaciones](https://charly-vibes.github.io/incitaciones/)** · [repo](https://github.com/charly-vibes/incitaciones): Colección de prompts reutilizables y buenas prácticas para herramientas CLI de LLMs. Se distribuyen como skills para Claude Code, Amp, Gemini CLI, Cursor, Windsurf y Zed. Recetas destiladas del delirio cotidiano.
*   **[canticos](https://charly-vibes.github.io/canticos/)** · [repo](https://github.com/charly-vibes/canticos): Cánticos, invocaciones, escrituras. Scripts de uso personal: conversión de video para proyector, transcripción con whisper, dashboard de uso de Claude Code. Herramientas pequeñas y afiladas.

### El laboratorio

Experimentos sin plan maestro. Fuegos de un día, prototipos y juguetes que quizás algún día encuentren su lugar. O no, y también está bien.



#### Aplicaciones web

*   **[atril](https://charly-vibes.github.io/atril/)** · [repo](https://github.com/charly-vibes/atril): Atril para el ecosistema wai. Visores web para leer specs e issues sin fricción, con foco en exploración cómoda desde tablet o navegador.
*   **[jams](https://charly-vibes.github.io/jams/)** · [repo](https://github.com/charly-vibes/jams): Pequeñas aplicaciones, fuegos de un día, para entender herramientas y modos de hacer directos, casi brutales. Cada app es una página, sin frameworks, sin ceremonias.
*   **[nayra](https://charly-vibes.github.io/nayra/)** · [repo](https://github.com/charly-vibes/nayra): Visualización de líneas de tiempo para el tiempo profundo. 10.000+ eventos a 60 FPS, desde microsegundos hasta miles de millones de años. Un intento de domesticar el caos con desarrollo guiado por especificaciones. Una jaula de oro para la creatividad.
*   **[superficies](https://charly-vibes.github.io/superficies/)** · [repo](https://github.com/charly-vibes/superficies): Catálogo de diseño para explorar dimensiones ortogonales de diseño web mediante vistas previas en vivo y exportación de informes deterministas.
*   **[tambor](https://charly-vibes.github.io/tambor/)** · [repo](https://github.com/charly-vibes/tambor): Librería de UI en TypeScript estricto, mobile-first: la UI es función pura del estado, los handlers son funciones puras que devuelven efectos y las combinaciones inválidas fallan en compile time. Port de membrane, con demo en vivo.
*   **[tRAGar](https://charly-vibes.github.io/tRAGar/)** · [repo](https://github.com/charly-vibes/tRAGar): Generación aumentada por recuperación (RAG) del lado del cliente en el navegador. Embeddings con transformers.js sin servidor.
*   **[wanna](https://charly-vibes.github.io/wanna/)** · [repo](https://github.com/charly-vibes/wanna): Arnés de conformancia spec-first para un sistema de interacción: el corpus specodelic es la fuente de verdad, cada propiedad está atada a un test de contrato ejecutable y los git hooks hacen imposible pushear un contrato en rojo.
*   **[miblioteca](https://charly-vibes.github.io/miblioteca/)** · [repo](https://github.com/charly-vibes/miblioteca): Captura de lomos de bibliotecas. Una PWA en TypeScript para catalogar libros a partir de fotos de sus lomos.

#### Mobile

*   **[paranoid](https://charly-vibes.github.io/paranoid/)** · [repo](https://github.com/charly-vibes/paranoid): Una app Android que aloja muchas apps pequeñas. Cada mini-app vive como una Activity nativa en Kotlin, con dependencias mínimas y bajo consumo de recursos.

#### Desktop

*   **[fotos](https://charly-vibes.github.io/fotos/)** · [repo](https://github.com/charly-vibes/fotos): Captura de pantalla con inteligencia artificial. Anotaciones visuales, análisis OCR, detección de PII y un servidor MCP para integración con agentes de código. El ojo que le faltaba al flujo de trabajo.

#### Otros experimentos

*   **[bichos](https://github.com/charly-vibes/bichos)** · [repo](https://github.com/charly-vibes/bichos): Framework bio-mimético para control de calidad autónomo. Enjambres de agentes especializados —hormigas, abejas, termitas, avispas— que coordinan por estigmergía para detectar bugs, analizar arquitectura y auditar seguridad.
*   **[khipu](https://github.com/charly-vibes/khipu)** · [repo](https://github.com/charly-vibes/khipu): Forensia de trazas de agentes y cristalización de flujos de trabajo. Una herramienta para desenredar hilos y encontrar patrones en el ruido.
*   **[ruta](https://github.com/charly-vibes/ruta)** · [repo](https://github.com/charly-vibes/ruta): Un paquete para pi que lo vuelve un arnés opinado para una semana de inmersión en especificaciones. Disciplina para no perderse en el entusiasmo de la máquina.
*   **[michael](https://charly-vibes.github.io/michael/)** · [repo](https://github.com/charly-vibes/michael): Tema de color solo en escala de grises para pantallas forzadas a monocromo: terminal, editores, e-ink. El significado viaja por luminosidad, peso y estilo, nunca por tono.
*   **[coffee](https://charly-vibes.github.io/coffee/)** · [repo](https://github.com/charly-vibes/coffee): Tracking de uso y costo de IA (Claude, Pi, Amp, Gemini). Extractor en Python y dashboards HTML autocontenidos: Gantt de multitasking, economía de suscripción, forecast.
*   **[paseos](https://github.com/charly-vibes/paseos)** · [repo](https://github.com/charly-vibes/paseos): Repo en gestación: todavía sin forma definida, solo la declaración de autoría y una intención que no se sabe qué va a ser cuando crezca.

### Distribución

Repositorios de paquetes para instalar las herramientas sin pelear con el toolchain: el tap de Homebrew, el bucket de Scoop y la submission a Flathub. La CLI dulce-de-leche (`ddl`), listada en el ecosistema, automatiza lo que estos repos exponen.

*   **[homebrew-charly](https://github.com/charly-vibes/homebrew-charly)** · [repo](https://github.com/charly-vibes/homebrew-charly): Tap de Homebrew para las herramientas de charly-vibes. Un `brew tap` y a trabajar.
*   **[scoop-charly](https://github.com/charly-vibes/scoop-charly)** · [repo](https://github.com/charly-vibes/scoop-charly): Bucket de Scoop para las herramientas de charly-vibes. Instalación directa en Windows.
*   **[flathub](https://github.com/charly-vibes/flathub)** · [repo](https://github.com/charly-vibes/flathub): Fork de flathub/flathub para el tracker de issues y la submission de fotos a Flathub. El trámite para llegar a las tiendas de Linux.

*Los repos meta —`charly-vibes` y `charly-vibes.github.io`— no se listan: su trabajo es describir al resto.*

---

Todo es parte de la misma pesquisa. Un diario de abordo en la era de la máquina que sueña. O de la máquina que nos hace soñar que estamos creando algo nuevo. Da igual. El viaje es lo único que cuenta.

---

## Nota sobre la autoría del código

Todo el código en este repositorio fue generado por un modelo de lenguaje de gran escala. Esto no es una confesión ni una disculpa. Es un dato, como el que dice que el agua hierve a cien grados a nivel del mar: neutro, técnico, y con consecuencias que uno descubre después.

Lo que hizo el humano es lo que suele hacerse antes y después de que sucedan las cosas: pensar. Revisar los requisitos, discutir los casos borde, entender qué se quiere construir y por qué, decidir cómo debería comportarse el sistema cuando la realidad —que es caprichosa y no lee documentación— lo enfrenta con situaciones imprevistas. Las horas de planificación, de diseño, de leer especificaciones hasta que el cansancio disuelve la frontera entre la comprensión y la alucinación.

El LLM escribe. El humano sabe qué debe decir.

Hay una distinción, aunque al mirar el historial de *commits* cueste encontrarla. La distinción está en que una máquina puede producir código correcto sin entender nada, del mismo modo que una calculadora puede resolver una integral sin saber qué es el tiempo. Entender para qué sirve eso, si realmente resuelve el problema, si el problema era el problema correcto: eso sigue siendo territorio humano. Por ahora.
