# Esponja bajo punzón

Simulador de una esponja cilíndrica seca, para estimar cómo responde un material esponjoso a la presión.

**Abrir:** https://rodrigo-svg.github.io/esponja-simulador/

## Qué incluye

- **Banco 2D (elementos finitos axisimétricos):** un punzón plano hunde el cilindro a 100 mm/min, se retira y la esponja se recupera. Curva fuerza–hundimiento, histéresis y recuperación en el tiempo.
- **Vista de poros:** toca una zona del corte para ver cómo se deforma y pandea cada poro según la carga local.
- **Ambiente:** la temperatura y la humedad cambian la rigidez del sólido y los tiempos de recuperación.
- **Ficha de material editable** para estimar otros materiales.

## Modelo

- Curva de espuma de Gibson–Ashby (elástica, meseta por pandeo de celdas, densificación).
- Hiperespuma de Storåkers con coeficiente de Poisson ajustable.
- Efecto Mullins (Ogden–Roxburgh) y viscoelasticidad de Prony.
- Humedad del sólido por isoterma GAB, transición vítrea por Gordon–Taylor y tiempos por WLF/Arrhenius.
- Criterio de ruptura por estiramiento máximo: marca dónde se desgarraría la espuma.

Verificado contra la compresión uniforme exacta y contra la solución de Boussinesq para punzón plano.

Todo corre en el navegador, en un solo archivo `index.html`.
