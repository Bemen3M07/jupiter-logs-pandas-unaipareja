## EXERCICI 1
**Explica quines comandes de Linux Pots fer servir a l’hora d’analitzar logs escrits a fitxer per a:**
**● Veure contínuament els logs que es van escrivint a un arxiu**
tail -f nom_fitxer.log

**● Cercar una paraula concreta dintre d’un arxiu de log**
grep "paraula" nom_fitxer.log


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


## EXERCICI 3

**PANDAS**
Pandas és una llibreria de Python molt popular i utilitzada per a l'anàlisi i manipulació de dades. Permet llegir, escriure i transformar dades en formats com CSV, JSON, Excel, i altres. Pandas facilita la neteja, manipulació, agrupament i càlcul estadístic de les dades, proporcionant estructures de dades com el DataFrame i Series.

**Funcionalitats clau:**

- Lectura i escriptura de fitxers en diversos formats (CSV, JSON, Excel).
- Filtratge, agrupament i agregació de dades.
- Tractament de valors nuls.
- Funcions estadístiques com mitjanes, sumes, etc.
- Visualització bàsica de dades (com gràfiques).

**Exemple bàsic amb Pandas:**

import pandas as pd

df = pd.read_csv('dades.csv')

print(df.head())

mitjana = df['columna_dades'].mean()
print(f'Mitjana: {mitjana}')


**JUPYTER NOTEBOOK**
Jupyter Notebook és una eina interactiva que permet escriure i executar codi Python de manera interactiva, juntament amb text, imatges i gràfiques. És ideal per a l'anàlisi de dades, ja que permet veure els resultats immediatament i visualitzar gràfiques a mesura que es desenvolupen les operacions.

**Funcionalitats clau:**

- Execució interactiva de codi Python.
- Visualització de resultats en línia (com gràfiques o taules).
- Integració amb llibreries com Pandas, Matplotlib, i altres per generar visualitzacions.
- Documentació i explicacions juntament amb el codi.
- Exemple d'ús amb Pandas i gràfics:

import pandas as pd
import matplotlib.pyplot as plt

df = pd.read_csv('dades.csv')

df['columna_dades'].plot(kind='bar')
plt.show()


**REPORTLAB**

ReportLab és una llibreria que permet generar documents PDF de manera programàtica. Es pot utilitzar per crear informes, cartes o qualsevol tipus de document PDF, incloent gràfiques generades a partir de les dades.

**Funcionalitats clau:**

- Creació de documents PDF des de zero.
Suport per a text, imatges i gràfiques en els PDFs.
Personalització dels dissenys dels informes (fonts, colors, marges, etc.).
Exemple d'ús amb ReportLab:

from reportlab.lib.pagesizes import letter
from reportlab.pdfgen import canvas

# Crear un PDF
c = canvas.Canvas("informe.pdf", pagesize=letter)
c.drawString(100, 750, "Informe de Dades")
c.save()


## EXERCICI 4


