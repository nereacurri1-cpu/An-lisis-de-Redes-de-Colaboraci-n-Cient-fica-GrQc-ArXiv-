# 📚 Análisis de Redes de Colaboración Científica (arXiv GrQc)

Este proyecto realiza un análisis completo y reproducible de la red de coautorías del dominio **Relatividad General y Cosmología Cuántica (GrQc)** del repositorio arXiv.  
El objetivo es estudiar la estructura de la comunidad científica mediante herramientas de **análisis de redes**, **detección de comunidades** y **visualización interactiva**.

---

## 🔍 Objetivos del proyecto

- Construir la red de colaboraciones científicas a partir de datos de coautoría  
- Identificar autores centrales y su rol estructural.  
- Detectar **comunidades científicas** usando el algoritmo Louvain.  
- Visualizar el gráfico completo y el subgrafo de los autores más influyentes.  
- Extraer conclusiones interpretadas basadas en teoría de redes.

---

## 🧠 Metodología

El análisis se desarrolla en Python utilizando:

- **NetworkX** para modelados, métricas y subgrafos  
- **Pandas** para manejo del conjunto de datos  
- **Matplotlib** para histogramas  
- **python-louvain** para detección de comunidades  
- **PyVis** para visualización dinámica e interactiva  

El cuaderno incluye:

1. Carga del conjunto de datos  
2. Exploración inicial y verificación de calidad  
3. Limpieza y preparación de datos  
4. Construcción del gráfico no dirigido  
5. Extracción del **LCC (Largest Connected Component)**  
6. Distribución de grado  
7. Construcción del subgrafo Top-500 autores  
8. Centralidades:  
   - Grado  
   - Intermediación  
   - Cercanía  
   - Vector propio  
   - PageRank  
9. Detección de comunidades (Lovaina)  
10. Visualización interactiva (PyVis)  
11. Exportación de métricas  
12. Conclusiones finales  

---

## 📈 Principales hallazgos

- La red presenta un **componente gigante (LCC)** con la mayoría de autores conectados.  
- La **distribución de grado es altamente sesgada**, con pocos hubs muy conectados.  
- Las centralidades permiten identificar:  
  - autores influyentes,  
  - autores puente,  
  - autores con prestigio estructural.  
- Las comunidades detectadas con Louvain revelan **subgrupos temáticos claros**.  
- La visualización interactiva PyVis muestra la **modularidad** y la estructura de clusters.  

---

## 🧩 Visualizaciones

El cuaderno genera:

- Histogramas de distribución de grados  
- Gráficos coloreados por la comunidad  
- Gráficos escalados por centralidad de grado  
- Un **mapa interactivo** descargable como HTML para explorar la red  

---

## 📁 Archivos incluidos

- `Analisis_de_Redes_de_colaboracion_cientifica.ipynb` — Cuaderno completo con análisis y visualizaciones  
- `top100_authors_centralities_sub500.csv` — Tabla con los autores más influyentes  
- `communities_partition_sub500.csv` — Comunidades detectadas  
- Carpeta `data/` con el dataset fuente (opcional)  
- `requirements.txt` — Dependencias para reproducir el proyecto  

---

## ▶️ Cómo ejecutar el proyecto

1. Clonar este repositorio:

```bash
clon de git https://github.com/USUARIO/analisis-redes-colaboracion-cientifica.git
