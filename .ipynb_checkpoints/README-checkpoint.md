## Comparació de llibreries de logging en diferents llenguatges

| **Característica**               | **Python**                      | **Java**                         | **Altres (opcional): JavaScript** |
|-----------------------------------|----------------------------------|-----------------------------------|------------------------------------|
| **Llenguatge**                    | Python                          | Java                             | JavaScript                        |
| **Nom de la llibreria**           | `logging`                       | `Log4j`                          | `Winston`                         |
| **És nativa del llenguatge?**     | Sí                              | No                               | No                                |
| **URL per descarregar la llibreria** | Inclosa en la biblioteca estàndard | [Log4j (Apache)](https://logging.apache.org/log4j/2.x/) | [Winston GitHub](https://github.com/winstonjs/winston) |
| **Inicialització de l’objecte de logger** | `logger = logging.getLogger()`   | `Logger logger = LogManager.getLogger();` | `const logger = require('winston');` |
| **Nivells de log disponibles**    | `DEBUG`, `INFO`, `WARNING`, `ERROR`, `CRITICAL` | `TRACE`, `DEBUG`, `INFO`, `WARN`, `ERROR`, `FATAL` | `error`, `warn`, `info`, `verbose`, `debug`, `silly` |
| **Mètode per fer log**            | `logger.info("Missatge")`       | `logger.info("Missatge")`        | `logger.info("Missatge");`        |
| **Tipus de manegadors**           | `StreamHandler` (pantalla), `FileHandler` (fitxer), etc. | `ConsoleAppender`, `FileAppender`, etc. | `Console` (pantalla), `File` (fitxer), etc. |
| **Opcions de format**             | `%time`, `%levelname`, `%message` | `PatternLayout` amb `%d`, `%p`, `%m`, etc. | JSON o formats personalitzats (`template`) |
