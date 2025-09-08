# 📊 Anime Recommendation Database 2020  

Este repositorio utiliza el dataset [Anime Recommendation Database 2020](https://www.kaggle.com/datasets/CooperUnion/anime-recommendations-database), que contiene información de **17,562 animes** y las preferencias de **325,772 usuarios**.  

# Contenido  

## Anime.csv  
- **anime_id** → ID único en *myanimelist.net* que identifica un anime.  
- **name** → Nombre completo del anime.  
- **genre** → Lista separada por comas con los géneros de este anime.  
- **type** → Tipo (película, TV, OVA, etc.).  
- **episodes** → Número de episodios (1 si es película).  
- **rating** → Calificación promedio del anime (escala de 1 a 10).  
- **members** → Número de miembros de la comunidad que forman parte del grupo de este anime.  

## Rating.csv  
- **user_id** → ID de usuario generado aleatoriamente (no identificable).  
- **anime_id** → ID del anime que este usuario ha calificado.  
- **rating** → Calificación otorgada (escala de 1 a 10; valor **-1** si el usuario vio el anime pero no asignó calificación).  

# Inspiración  
Construir un sistema de recomendación de anime más efectivo, basado únicamente en el historial de visualización de los usuarios.  


# Metodología

1.  **Exploración de datos**: análisis de calificaciones, géneros y
    estados de visionado.\
2.  **Preparación y limpieza**: manejo de valores nulos y transformación
    de variables.\
3.  **Modelado**: implementación de varios enfoques (item, contenido y deep learning

# Conclusiones 
Ningún modelo es “mejor” sólo por la cantidad de recomendaciones (porque es fija).

La evaluación debería basarse en métricas como precisión, recall, NDCG, MAP o satisfacción del usuario.

Lo interesante del DataFrame es que permite comparar cuáles títulos coinciden entre métodos y cuáles son exclusivos de cada enfoque, en este caso no se encontró intersecciones. Lo que no indica que tenemos que ampliar la muestra dado que en este ejercicio se tomo el 10% de las recomendaciones por limitaciones computacionales.
