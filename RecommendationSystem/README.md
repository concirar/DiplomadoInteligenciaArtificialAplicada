# 📊 Anime Recommendation Database 2020  

Este repositorio utiliza el dataset [Anime Recommendation Database 2020](https://www.kaggle.com/datasets/hernan4444/anime-recommendation-database-2020/data), que contiene información de **17,562 animes** y las preferencias de **325,772 usuarios**.  

## 📁 Contenido del dataset  

El dataset incluye:  

- **Lista de animes por usuario**: incluye estados como *completado, en curso, en pausa, abandonado y planeado*.  
- **Calificaciones** dadas por los usuarios a los animes que han visto completamente.  
- **Información general del anime**: géneros, estadísticas, estudios, etc.  
- **Archivos HTML** con información scrappeada de MyAnimeList (reseñas, sinopsis, staff, estadísticas, etc.).  
- **Código de recolección de datos** disponible en [este repositorio](https://github.com/Hernan4444/MyAnimeList-Database).  

⚠️ **Advertencia**: el dataset incluye información sobre anime para adultos (*hentai*).  

Los datos fueron recolectados entre el **26 de febrero y el 20 de marzo de 2020**.  

---

## 📂 Archivos principales  

- **`animelist.csv`**  
  Contiene la lista de animes registrados por los usuarios con su respectiva puntuación, estado y episodios vistos.  
  - 109 millones de filas  
  - 17,562 animes  
  - 325,772 usuarios  

  **Columnas**:  
  - `user_id`: identificador anónimo del usuario.  
  - `anime_id`: ID de MyAnimeList del anime.  
  - `score`: puntuación del 1 al 10 (0 si no asignó).  
  - `watching_status`: estado del anime en la lista del usuario.  
  - `watched_episodes`: número de episodios vistos.  

- **`watching_status.csv`**  
  Diccionario de estados posibles para la columna `watching_status`.  

- **`rating_complete.csv`**  
  Subconjunto de `animelist.csv` con animes **completados y calificados**.  
  - 57 millones de calificaciones  
  - 16,872 animes  
  - 310,059 usuarios  

  **Columnas**:  
  - `user_id`  
  - `anime_id`  
  - `rating`  

- **`anime.csv`**  
  Información general de los animes (17,562 entradas), incluyendo:  
  - Nombre en inglés y japonés  
  - Géneros  
  - Tipo (TV, OVA, Película, etc.)  
  - Número de episodios  
  - Fecha de emisión  
  - Estudios, productores y licenciatarios  
  - Fuente (manga, novela ligera, original, etc.)  
  - Puntuación promedio  
  - Estadísticas de popularidad y favoritos  
  - Distribución de calificaciones (score 1–10)  

- **Carpeta `html/`**  
  Contiene **1 archivo ZIP por anime** con páginas extraídas de MyAnimeList:  
  - Página principal  
  - Reseñas  
  - Recomendaciones  
  - Estadísticas  
  - Personajes y Staff  

  ⚠️ Debido al tamaño, los archivos HTML completos están disponibles en [Google Drive](https://drive.google.com/drive/folders/12ghJk-sWyXXORoLBUpPirK4YdtIaZPV_?usp=sharing).  

---

## 🙏 Agradecimientos  

- [MyAnimeList](https://myanimelist.net/) por proveer la información.  
- [Jikan API](https://jikan.moe/) por acceso a preferencias de usuarios.  
- Pontificia Universidad Católica de Chile por los servidores para la recolección de datos.  

---

## 💡 Inspiración  

Este dataset permite:  

- Realizar **ejercicios de scraping** con los HTML descargados.  
- Construir y probar diferentes **sistemas de recomendación de anime**:  
  - Filtrado colaborativo.  
  - Recomendaciones basadas en contexto (género, staff, reseñas, sinopsis, etc.).  
- Analizar qué características contribuyen a un mejor sistema de recomendación.  

---

## 🚀 Ideas futuras  

- Ampliar el dataset a **mangas y novelas**.  
