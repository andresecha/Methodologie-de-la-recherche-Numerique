# 🎙️ Speech-to-text Whisper

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **🌍 Bilingual Repository / Dépôt Bilingue / Repositorio Bilingüe**
> - [🇫🇷 Lire en Français](#-français)
> - [🇪🇸 Leer en Español](#-español)

---

## 🇫🇷 Français

### Guide Méthodologique pour la Transcription Automatique de l'Audio avec Whisper (OpenAI)

Ce dépôt contient un environnement de travail basé sur un carnet Jupyter (Google Colab) conçu pour transformer les sources sonores en textes exploitables pour la recherche.

Une part considérable de la production intellectuelle, patrimoniale et testimoniale des sciences humaines et sociales n'existe que sous forme orale (entretiens de terrain, conférences, fonds sonores). Ces matériaux constituent des sources primaires d'une valeur inestimable, mais demeurent largement inaccessibles à la recherche plein texte tant qu'ils n'ont pas fait l'objet d'une transcription. Ce projet automatise et optimise ce processus.

### ⚙️ Fonctionnalités Principales

| Capacité | Description | Intérêt pour la recherche |
| :--- | :--- | :--- |
| **Transcription** | Convertit la parole en texte dans la langue d'origine. | Produire des versions textuelles d'entretiens ou de témoignages. |
| **Traduction** | Traduit l'audio de n'importe quelle langue vers l'anglais. | Faciliter l'accès à des sources dans des langues non maîtrisées. |
| **Détection** | Identifie automatiquement la langue parlée. | Classer des fonds sonores multilingues sans écoute préalable. |

### 🛠️ Architecture et Flux de Travail

Le carnet est structuré logiquement par phases de traitement :
1. **Configuration et Dépendances :** Activation du GPU (T4 recommandé) et installation de `openai-whisper`, `ffmpeg` et `yt-dlp`.
2. **Sélection des Modèles :** Évaluation du rapport qualité / vitesse / VRAM (de `tiny` à `large` et `turbo`).
3. **Acquisition des Données (3 voies) :** - Téléversement local.
   - Connexion directe avec Google Drive.
   - Extraction audio depuis YouTube.
4. **Traitement (CLI ou Python) :** Transcription avec paramètres ajustables (vocabulaire spécialisé, horodatage précis).
5. **Exportation :** Génération de formats structurés (`.txt`, `.srt`, `.vtt`, `.tsv`, `.json`).

### 🚀 Utilisation Rapide (Ligne de Commandes)

```bash
# Transcription de base, qualité maximale
whisper "audio.mp3" --model large --language French --output_format all --output_dir /resultats

# Transcription rapide pour fichiers longs
whisper "audio.mp3" --model turbo --language French --output_format all --output_dir /resultats
```

### 📝 Citation
> Echavarría, Andrés. *Guide méthodologique pour la transcription automatique de l'audio avec Whisper (OpenAI)*. Groupe d'intérêt « Acquisition assitée de textes », Consortium Huma-Num ARIANE. [Carnet Jupyter Google Colab], version 1.0, mars 2026.

---

## 🇪🇸 Español

### Guía Metodológica para la Transcripción Automática de Audio con Whisper (OpenAI)

Este repositorio contiene un entorno de trabajo basado en un cuaderno Jupyter (Google Colab) diseñado para transformar fuentes sonoras en textos explotables para la investigación.

Una parte considerable de la producción intelectual, patrimonial y testimonial en las ciencias humanas y sociales existe únicamente en formato oral (entrevistas, conferencias, archivos sonoros). Estas fuentes primarias son invaluables, pero permanecen inaccesibles para búsquedas de texto completo o análisis textual sin una transcripción adecuada. Este proyecto automatiza y optimiza dicho proceso.

### ⚙️ Capacidades Principales

| Capacidad | Descripción | Interés para la Investigación |
| :--- | :--- | :--- |
| **Transcripción** | Convierte voz a texto en el idioma original. | Generar versiones textuales de entrevistas y conferencias. |
| **Traducción** | Traduce el audio de cualquier idioma al inglés. | Facilitar el acceso preliminar a fuentes en idiomas no dominados. |
| **Detección** | Identifica automáticamente el idioma hablado. | Clasificar archivos sonoros multilingües sin escucha previa. |

### 🛠️ Arquitectura y Flujo de Trabajo

El cuaderno está estructurado lógicamente por fases de procesamiento:
1. **Configuración y Dependencias:** Activación de GPU (T4 recomendado) e instalación de `openai-whisper`, `ffmpeg` y `yt-dlp`.
2. **Selección de Modelos:** Evaluación del equilibrio entre calidad, velocidad y consumo de VRAM (desde `tiny` hasta `large` y `turbo`).
3. **Ingesta de Datos (3 vías):** - Carga local de archivos.
   - Conexión directa con Google Drive.
   - Extracción de audio desde YouTube.
4. **Procesamiento (CLI o Python):** Transcripción con parámetros ajustables (diccionarios especializados, marcas de tiempo precisas).
5. **Exportación:** Generación de formatos estructurados (`.txt`, `.srt`, `.vtt`, `.tsv`, `.json`).

### 📝 Cita
> Echavarría, Andrés. *Guía metodológica para la transcripción automática de audio con Whisper (OpenAI)*. Grupo de interés «Acquisition assitée de textes», Consortium Huma-Num ARIANE. [Cuaderno Jupyter Google Colab], versión 1.0, marzo de 2026.

---

*Développé avec ❤️ et ☕ pour la communauté des Humanités Numériques.*


*Desarrollado con ❤️ y ☕ para la comunidad de Humanidades Digitales.*
