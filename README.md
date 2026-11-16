# NatoMetrix

Herramienta web para los informes de **autopsias fetales y perinatales**. Funciona en catalán, castellano e inglés.

Introduces la edad gestacional, las medidas y los pesos, y NatoMetrix:

- compara cada valor con tablas de referencia (media ± DE, z, percentil y edad gestacional equivalente);
- marca lo que está significativamente alterado (criterio elegible: < P3 / > P97, < P5 / > P95 o ± 2 DE);
- genera las tablas para copiar en el informe, con las columnas que elijas;
- redacta el texto del informe y la frase de la epicrisis (pesos, medidas y retención).

**Web:** se abre `index.html` en cualquier navegador. Si el repositorio tiene activado GitHub Pages, está en `https://<usuario>.github.io/natometrix/`.

## Apartados

- **Datos del caso:** número de necropsia, fecha, residente, patólogo/a, tipo de caso (ILE, MFIU, muerte neonatal, aborto), gestación única o múltiple y corionicidad, sexo y edad gestacional.
- **Pesos de órganos:** cada órgano tiene un estado (pesado, por debajo del rango de la báscula, ausente/agenesia, no pesado) y una casilla de fijado en formol. Los órganos pares se registran por lado y en conjunto.
- **Medidas externas**, otras medidas y huesos largos.
- **Ratios:** encéfalo/hígado, pulmones/peso corporal y cráneo-sacra/cráneo-caudal; en gestación múltiple, la discordancia de peso entre fetos.
- **Restricción del crecimiento:** percentiles de Bartosch y peso personalizado de Figueras. De Figueras solo está activo el modelo a término; el resto queda pendiente de validar.
- **Placenta y cordón:** peso según el tipo de gestación, cociente peso fetal/placentario, cordón (longitud, diámetro, coiling index, inserción, vasos) y membranas.
- **Tiempo de muerte intrauterina** (Genest 1992): hallazgos externos, histología fetal e histología placentaria, comparados con el intervalo clínico.
- **Epicrisis:** apertura, hallazgos, pesos y medidas, retención y número de biopsia de la placenta.

## Datos y privacidad

- **No introduzcas datos identificativos de pacientes:** ni nombres, ni NHC, ni DNI/CIP. Identifica cada caso solo con el número de necropsia.
- **Dónde se guardan los casos:** solo en el navegador del ordenador donde se introducen (`localStorage`). No se envían a ningún servidor ni a GitHub.
- **Cuándo se pierden:** si se borran los datos de navegación o se cambia de ordenador. Usa **Exportar casos** a menudo para tener una copia de seguridad (un archivo `.json`), e **Importar casos** para recuperarla o pasarla a otro ordenador.
- **Nunca subas los archivos exportados a este repositorio.** El `.gitignore` ya los excluye.
- **Lectura de fotos de la plantilla:** esta versión no la incluye, porque requiere un servicio de IA con cuenta. Existe solo en la versión de claude.ai.

## Referencias

- Bartosch C, et al. Fetal autopsy parameters standards: biometry, organ weights, and long bone lengths. *Virchows Arch* 2019;475:499–511.
- Pinar H, et al. Reference values for singleton and twin placental weights. *Pediatr Pathol Lab Med* 1996;16:901–7.
- Hecht JL, et al. Reference weights for placentas delivered before the 28th week of gestation. *Placenta* 2007;28:987–90.
- Pinar H, et al. Triplet placentas: reference values for weights. *Pediatr Dev Pathol* 2002;5:495–8.
- Heerema-McKenney A. *Diagnostic Pathology: Placenta*, 2nd ed. Elsevier, 2018.
- Machin GA, Ackerman J, Gilbert-Barness E. Abnormal umbilical cord coiling is associated with adverse perinatal outcomes. *Pediatr Dev Pathol* 2000;3:462–71.
- Genest DR, et al. Estimating the time of death in stillborn fetuses (I, II, III). *Obstet Gynecol* 1992;80:575–600.
- Johnson P, Maxwell D. Fetal penile length. *Ultrasound Obstet Gynecol* 2000;15:308–10.
- Allanson JE, et al. / Hennekam RCM, et al. Elements of morphology. *Am J Med Genet A* 2009;149A.
- Figueras F, et al. Customized birthweight standards for a Spanish population. *Eur J Obstet Gynecol Reprod Biol* 2008;136:20–4.
- Cociente peso fetal/placentario: percentiles de Baystate Medical Center (15.463 partos).

## Aviso

NatoMetrix es una ayuda para redactar informes, no un producto sanitario. Los valores, percentiles y frases que genera deben revisarse siempre antes de incorporarlos a un informe. Las tablas se han transcrito a mano de las fuentes citadas: si encuentras un error, abre un *issue*.

Los temas pendientes están en [`docs/PENDENTS.md`](docs/PENDENTS.md).

---

*De Xandre para os resis que sofren tanto as necros.*
