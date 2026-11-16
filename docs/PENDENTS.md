# NatoMetrix: temes pendents

## Figueras 2008: pes personalitzat

**Estat (5/11/2026):** a NatoMetrix hi ha un apartat «Restricció del creixement», amb els percentils de Bartosch i el pes òptim de Figueras a terme (37–42 setm.) i la desviació en %. El model a terme s'ha comprovat amb l'exemple de l'article (3453 g). Falta validar-lo amb la calculadora: introduir 3–4 casos inventats (28, 32, 36 i 40 setm., amb dades maternes diferents) i comparar-ne el pes esperat i el percentil.

**Referència:** Figueras F, Meler E, Iraola A, et al. *Customized birthweight standards for a Spanish population.* Eur J Obstet Gynecol Reprod Biol 2008;136:20–4. doi:10.1016/j.ejogrb.2006.12.015

**Què és:** un model de pes en néixer personalitzat (mètode Gardosi). Es va fer amb nascuts vius, sans i a terme (259–293 dies) de l'Hospital Clínic. No té taules de percentils ni d'òrgans.

**Model (taula 3).** La constant és la mare estàndard: 161 cm, 59 kg, europea, primípara, 280 dies.
- Constant: 3269,47 g
- Edat gestacional: +16,66 g/dia (respecte de 280 dies)
- Paritat: para 1 +97,93 · para 2 +127,02 · para 3+ +152,29
- Ètnia: Àsia oriental +83,32 · Marroc +73,83 · Sud-Amèrica +95,09
- Talla materna (respecte de 161 cm): lineal 8,768 · cúbic 0,008
- Pes matern (respecte de 59 kg): lineal 6,90 · quadràtic −0,12 · cúbic 0,001
- Sexe: ±51,79 (nen +, nena −)
- Tabac: −124 / −211 / −256. Normalment no s'ajusta.
- Exemple de l'article: mateixa mare, tercer embaràs, 64 kg → 3453 g

**Comparació amb Bartosch (pes corporal, mare estàndard, mitja setmana):**

| EG | Bartosch | Figueras | Diferència |
|---|---|---|---|
| 37 | 2612 ± 411 g | 2970 g | −12 % |
| 38 | 2804 ± 439 g | 3086 g | −9 % |
| 39 | 3000 ± 467 g | 3203 g | −6 % |
| 40 | 3202 ± 496 g | 3319 g | −4 % |
| 41 | 3408 ± 526 g | 3436 g | ≈ 0 % |

**Què falta per implementar-ho bé:**
1. La corba de proporcionalitat (Hadlock / GROW) per aplicar-lo abans de les 37 setmanes.
2. El coeficient de variació del model, per poder passar a percentils.
3. Com ho calcula la calculadora de Medicina Fetal Barcelona.
4. Decidir si s'aplica a fetus morts, tenint en compte la pèrdua de pes per retenció i maceració.

## Altres pendents
- **Graus de maceració:** decidir l'escala o substituir-la pel mòdul de Genest.
- **Punts de tall de les ràtios:** encèfal/fetge ≥ 4; pulmó/pes < 0,015 abans de les 28 setmanes i < 0,012 a partir de les 28.
- **Coiling del cordó:** ara surt en anglès als tres idiomes (coiling index, hypocoiling, hypercoiling). Cal consultar el terme català. Opcions: espiralització, enrotllament, girat; s'ha desaconsellat «torsió» perquè es confon amb la torsió del cordó.
- **Termes en català de la placenta:** confirmar circummarginada i circumval·lada. Els de Genest ja estan confirmats: descamació o despreniment cutani, momificació, cariorrexi, pell marró/fosca.
- **Valors poc llegibles de la taula III de Genest:** revisar-los a l'original.

## Descartat
- **Diàmetres orbitaris i mesures del cor:** no se solen informar; del cor només se'n dona el pes.
