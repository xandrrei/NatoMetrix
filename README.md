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

- **NatoMetrix no guarda ningún caso.** Todo lo que se introduce se borra al cerrar o recargar la página: no se guarda en el navegador, ni se envía a ningún servidor, ni llega a GitHub.
- Para conservar los resultados, cópialos al informe con los botones de copiar.
- **No introduzcas datos identificativos de pacientes:** ni nombres, ni NHC, ni DNI/CIP.
- Lo único que recuerda el navegador son preferencias de uso (idioma, columnas que se copian, modo de los órganos pares), que no contienen datos de pacientes.
- **Lectura de fotos de la plantilla:** esta versión no lee fotos directamente, porque haría falta un servicio de IA con cuenta. En su lugar, usa **«Omplir des d'un text»**:
  1. pulsa «Copiar instruccions per a la IA»;
  2. pega las instrucciones en tu IA (Claude, Copilot…) junto con la foto;
  3. copia la respuesta y pégala en NatoMetrix, que rellena las casillas y marca en amarillo los valores para revisar.

  También se puede escribir el texto a mano con el mismo formato (`Pes: 585 g`, `Cervell: 82 g`, `PD: 8,5 g | PI: 7,2 g`…). La foto se sube a la IA de cada persona: que no salgan datos identificativos.

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
