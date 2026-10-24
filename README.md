# Desafío Mercado Central de San Salvador (DMD404)

**Integrantes:** 1. Kenneth Jeshua González Sosa - GS250179
                 2. Sebastián Enrique Colocho Jiménez - CJ252435
                 
**Fecha:** 24/10/2026
**Curso:** Datawarehouse y Minería de Datos (DMD404), Universidad Don Bosco

## Descripción
Análisis de datos para la reactivación económica del Mercado Central de San Salvador
con tres técnicas: reglas de asociación (Apriori), segmentación con K-Means y
predicción de quiebra con árbol de decisión.

#. Estructura del repositorio
- `desafio_mercado_central.ipynb`: cuaderno con los tres retos, ejecutado de principio a fin.
- `datasets/`: los 3 CSV originales, sin modificar.
- `output/`: `top_lift.png`, `kmeans_clusters.png`, `decision_tree.png`.
- `informe_tecnico.pdf`: informe de 2 páginas.
- `respuestas_reflexion.md`: respuestas a las preguntas de reflexión crítica.
- `requirements.txt`: versiones exactas de las bibliotecas.

# Cómo reproducir
1. `pip install -r requirements.txt`
2. Colocar los CSV en `datasets/`.
3. Ejecutar el cuaderno completo (semilla aleatoria 42 en todos los modelos).

# Resultados principales
- **Reto 1:** kit de productos del hogar (lift ≈ 14.7) y pares como maíz blanco ↔ loroco.
- **Reto 2:** 3 segmentos de comerciantes (K=3, estructura débil, silueta ≈ 0.13).
- **Reto 3:** árbol con AUC ≈ 0.69 en validación cruzada; la caída de ingresos es el mejor predictor.
