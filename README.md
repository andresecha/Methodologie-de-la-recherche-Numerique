# 📚 Metodología de la Investigación Digital / Méthodologie de la Recherche Numérique

Este repositorio reúne guías metodológicas y entornos de trabajo basados en cuadernos Jupyter (Google Colab) diseñados para investigadores en **Ciencias Humanas y Sociales (CHS)**. El objetivo es facilitar la transformación de fuentes primarias (documentos impresos, manuscritos y archivos sonoros) en datos textuales estructurados y explotables.

Este proyecto es desarrollado en el marco del **Grupo de interés en adquisición asistida de textos** del **Consorcio Huma-Num ARIANE**.

---

## 🛠️ Herramientas Disponibles

| Herramienta | Descripción | Acceso |
| :--- | :--- | :--- |
| **[OCR con Mistral AI](./OCR/Mistral/)** | Extracción de texto, tablas y LaTeX desde PDFs complejos y manuscritos. | [Guía ES](./OCR/Mistral/Metodological_guide_MistralOCR_Transcripcion_ARIANE_ES.ipynb) / [Guía FR](./OCR/Mistral/Metodological_guide_MistralOCR_Transcripcion_ARIANE_FR.ipynb) |
| **[Speech-to-Text con Whisper](./Speech-to-text/Whisper/)** | Transcripción y traducción automática de audio (entrevistas, archivos sonoros). | [Guía ES](./Speech-to-text/Whisper/Metodological_guide_Whisper_audio_Transcripcion_ARIANE_ES.ipynb) / [Guía FR](./Speech-to-text/Whisper/Metodological_guide_Whisper_audio_Transcripcion_ARIANE_FR.ipynb) |

---

## ⚖️ Licencias y Condiciones de Uso

### 1. Licencia del Proyecto
El código y las guías de este repositorio se distribuyen bajo la licencia **GNU General Public License v3 (GPLv3)**. Esto permite su uso, modificación y distribución libre, siempre que se mantenga la misma licencia y se reconozca la autoría.

### 2. Servicios de Terceros
El uso de estas herramientas implica la interacción con servicios externos cuyos términos de servicio el usuario debe conocer y aceptar:
*   **Mistral AI:** El uso del modelo `mistral-ocr-latest` requiere una clave API personal y está sujeto a los [Términos de Servicio de Mistral AI](https://mistral.ai/terms/).
*   **OpenAI Whisper:** El modelo Whisper es de código abierto (Licencia MIT), pero su implementación en estos cuadernos puede requerir el cumplimiento de las [Políticas de Uso de OpenAI](https://openai.com/policies/usage-policies) si se utiliza su infraestructura de API.

### 3. Responsabilidad y Privacidad
*   **Datos Sensibles:** El usuario es responsable de no subir documentos o audios que contengan datos personales sensibles a infraestructuras de terceros sin el debido consentimiento o anonimización previa.
*   **API Keys:** Nunca compartas tus claves API ni las incluyas en versiones públicas de tus cuadernos.

---

## 📝 Citación

Si utilizas estas guías en tu investigación, por favor utiliza las siguientes referencias:

- **Para Mistral OCR:** Echavarría, A.; Roulet, T. *Guía metodológica para el reconocimiento óptico de documentos con Mistral OCR*. Consorcio Huma-Num ARIANE, 2026.
- **Para Whisper:** Echavarría, A. *Guía metodológica para la transcripción automática de audio con Whisper*. Consorcio Huma-Num ARIANE, 2026.

---

*Desarrollado con ❤️ y ☕ para la comunidad de Humanidades Digitales.*
