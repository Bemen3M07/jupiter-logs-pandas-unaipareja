## EXERCICI 1
**Explica quines comandes de Linux Pots fer servir a l’hora d’analitzar logs escrits a fitxer per a:**
**● Veure contínuament els logs que es van escrivint a un arxiu**
tail -f nom_fitxer.log

**● Cercar una paraula concreta dintre d’un arxiu de log**
grep "paraula" nom_fitxer.log


## EXERCICI 2.1


## EXERCICI 2.2
## Què és millor, mostrar els logs a la terminal durant l'execució del programa o bolcar-los en un fitxer de text?

Depèn de l'ús i dels objectius del sistema:

- **Mostrar els logs a la terminal durant l'execució** és útil durant el desenvolupament i la depuració del programa. Permet obtenir informació en temps real sobre el comportament del sistema i facilita la identificació immediata de problemes.
  
- **Bolcar els logs en un fitxer de text** és ideal per a sistemes en producció. Això permet conservar un registre persistent dels esdeveniments que es poden analitzar posteriorment, especialment en casos d'errors o investigacions posteriors.


## EXERCICI 2.3



## Comparació de llibreries de logging en diferents llenguatges

| **Característica**               | **Python**                      | **Java**                         | **JavaScript**                    |
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


## EXERCICI 2.4

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


