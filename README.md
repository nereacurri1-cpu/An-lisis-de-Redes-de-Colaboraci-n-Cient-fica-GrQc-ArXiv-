# 📚 Análisis de Redes de Colaboración Científica (arXiv GrQc)

Este proyecto realiza un análisis completo y reproducible de la red de coautorías del dominio **General Relativity and Quantum Cosmology (GrQc)** del repositorio arXiv.  
El objetivo es estudiar la estructura de la comunidad científica mediante herramientas de **análisis de redes**, **detección de comunidades** y **visualización interactiva**.

---

## 🔍 Objetivos del proyecto

- Construir la red de colaboraciones científicas a partir de datos de coautoría.  
- Identificar autores centrales y su rol estructural.  
- Detectar **comunidades científicas** usando el algoritmo Louvain.  
- Visualizar el grafo completo y el subgrafo de los autores más influyentes.  
- Extraer conclusiones interpretadas basadas en teoría de redes.

---

## 🧠 Metodología

El análisis se desarrolla en Python utilizando:

- **NetworkX** para modelado, métricas y subgrafos  
- **Pandas** para manejo del dataset  
- **Matplotlib** para histogramas  
- **python-louvain** para detección de comunidades  
- **PyVis** para visualización dinámica e interactiva  

El notebook incluye:

1. Carga del dataset  
2. Exploración inicial y verificación de calidad  
3. Limpieza y preparación de datos  
4. Construcción del grafo no dirigido  
5. Extracción del **LCC (Largest Connected Component)**  
6. Distribución de grado  
7. Construcción del subgrafo Top-500 autores  
8. Centralidades:  
   - Degree  
   - Betweenness  
   - Closeness  
   - Eigenvector  
   - PageRank  
9. Detección de comunidades (Louvain)  
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

El notebook genera:

- Histogramas de distribución de grado  
- Grafos coloreados por comunidad  
- Grafos escalados por centralidad de grado  
- Un **mapa interactivo** descargable como HTML para explorar la red  

---

## 📁 Archivos incluidos

- `Analisis_de_Redes_de_colaboracion_cientifica.ipynb` — Notebook completo con análisis y visualizaciones  
- `top100_authors_centralities_sub500.csv` — Tabla con los autores más influyentes  
- `communities_partition_sub500.csv` — Comunidades detectadas  
- Carpeta `data/` con el dataset fuente (opcional)  
- `requirements.txt` — Dependencias para reproducir el proyecto  

---

## ▶️ Cómo ejecutar el proyecto

1. Clonar este repositorio:

```bash
git clone https://github.com/USUARIO/analisis-redes-colaboracion-cientifica.git
