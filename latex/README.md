# Electromagnetismo I — Tema 1: Leyes básicas de la electrostática

Apuntes formalizados (LaTeX) con el mismo estilo que el Tema 0 (*Herramientas matemáticas*).

## Compilación

```bash
cd latex
latexmk -pdf main.tex      # pdfLaTeX + biber (3 pasadas, ~3 min)
```

* Las líneas de campo y las equipotenciales de la figura 12 se calculan **dentro de TikZ** (integración numérica
  con `pgfmath`), sin datos externos; por eso la compilación completa tarda unos minutos.
* Para iterar rápido, crea un fichero vacío `latex/rapido.flag`: la figura de líneas de campo se sustituye por un
  marcador y la compilación baja a ~10 s. Bórralo para la compilación final.

## Estructura

| Fichero | Contenido |
|---|---|
| `main.tex`, `portada.tex`, `preambulo.tex` | Documento, portada y preámbulo (idénticos en estilo al Tema 0) |
| `secciones/01_introduccion.tex` | Contexto histórico, límites de validez, cuatro fuerzas, teoría de campos |
| `secciones/02_coulomb.tex` | Carga, balanza de Coulomb, Cavendish, ley de Coulomb, superposición |
| `secciones/03_campo.tex` | Campo eléctrico, densidades de carga, distribuciones continuas |
| `secciones/04_gauss.tex` | Ángulo sólido, ley de Gauss (integral y diferencial), delta de Dirac, simetrías |
| `secciones/05_potencial.tex` | Potencial, trabajo, conservatividad, Helmholtz, Poisson/Laplace, líneas de campo |
| `secciones/06_contorno.tex` | Condiciones de contorno de $\vec F$, $\vec E$ y $\phi$ |
| `secciones/07_seminarios.tex` | Problemas 1.1–1.12 resueltos |
| `secciones/08_apendice.tex` | Significado físico de grad/div/rot, identidades y formulario |
| `figuras/` | Todas las figuras (TikZ / pgfplots) |
| `referencias.bib` | Bibliografía |
