# 📊 Anime Recommendation Database 2020  

Este repositorio utiliza el dataset [Anime Recommendation Database 2020](https://www.kaggle.com/datasets/hernan4444/anime-recommendation-database-2020/data), que contiene información de **17,562 animes** y las preferencias de **325,772 usuarios**.  

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

# Agradecimientos  
Gracias a la API de **myanimelist.net** por proporcionar los datos de anime y valoraciones de usuarios.  

# Inspiración  
Construir un sistema de recomendación de anime más efectivo, basado únicamente en el historial de visualización de los usuarios.  
---


