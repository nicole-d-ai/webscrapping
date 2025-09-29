# 🌐 Webscraping con sitio web

Este proyecto consiste en aplicar técnicas de **webscraping** y **procesamiento de lenguaje natural (PLN)** para analizar un texto extraído de un sitio web donde una autora comparte su opinión sobre el libro *Pasión* de Isabel Allende.  

## 📚 Librerías utilizadas

- `requests` → realizar peticiones HTTP  
- `beautifulsoup4` → parsear y navegar el HTML  
- `html5lib` → parser tolerante a HTML desordenado  
- `re` → expresiones regulares para limpieza de texto  
- `spacy` → tokenización, lematización y stopwords en español  
- `collections.Counter` → conteo de frecuencias  
- `matplotlib` → visualización  
- `wordcloud` → generar nubes de palabras  
- `scikit-learn` → `CountVectorizer` y `TfidfVectorizer` para vectorización  
- `numpy` → manipulación de matrices

## 📝 Pasos realizados

1. **Scraping**: descarga del HTML con `requests` y extracción de párrafos con `BeautifulSoup`.  
2. **Limpieza inicial**: eliminación de caracteres raros, espacios extra y oraciones vacías.  
3. **Procesamiento lingüístico** con `spaCy`:  
   - Tokenización  
   - Lematización  
   - Eliminación de *stopwords*  
   - Filtro de palabras cortas  
4. **Construcción de oraciones limpias**: cada oración = un documento.  
5. **Vectorización**:  
   - **CountVectorizer** → matriz documento–término con frecuencias.  
   - **TfidfVectorizer** → matriz con pesos TF-IDF que resaltan términos más relevantes.  
6. **Visualización**: nube de palabras y análisis de frecuencias.  

---

## 🎯 Objetivos

- Comprender cómo realizar **webscraping** para obtener texto desde un sitio web.  
- Aprender a **preprocesar texto** (limpieza, tokenización, lematización).  
- Generar una **representación numérica del texto** (matriz documento–vocabulario).  
- Analizar la **importancia de las palabras** con TF-IDF.  
- Visualizar resultados con una **nube de palabras**.  

---

## ✅ ¿Qué se logró?

- Se obtuvo un **texto limpio y normalizado** listo para análisis.  
- Se construyeron las matrices de **frecuencias** y **TF-IDF**.  
- Se identificaron los **términos más relevantes** del corpus.  
- Se comprendió el flujo completo: *scraping → limpieza → preprocesamiento → vectorización → visualización*.  

---

✨ Este trabajo muestra cómo pasar de un **texto en bruto de una web** a **datos numéricos listos para minería de texto**.
