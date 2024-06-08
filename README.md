# ChatBot_Alarms

`ChatBot_Alarms` es un proyecto que consiste en un chatbot diseñado para ayudar a los usuarios a verificar la cobertura de seguridad en sus códigos postales y proporcionar información sobre los servicios de alarma. El proyecto se compone de varias partes, incluidas carpetas de datos, scripts en Jupyter Notebook y archivos CSV para el manejo de la información.

## Estructura del Proyecto

- `codigos1220n/`: Carpeta que contiene 152 archivos .txt con todos los códigos postales y los barrios correspondientes de España.
- `BOT.ipynb`: Jupyter Notebook que implementa la lógica principal del chatbot.
- `Bot Machine Learning.ipynb`: Jupyter Notebook para implementar algoritmos de aprendizaje automático relacionados con el chatbot.
- `CP_generator.ipynb`: Jupyter Notebook que genera un archivo CSV con los códigos postales y su cobertura.
- `cobertura.csv`: Archivo CSV que contiene la cobertura de los códigos postales.
- `registros.csv`: Archivo CSV que almacena los datos de los usuarios que interactúan con el chatbot.

## Descripción de los Jupyter Notebooks

### CP_generator.ipynb

Este script lee los archivos de texto en la carpeta `codigos1220n` y extrae los códigos postales y localidades. Luego, genera una cobertura aleatoria para cada entrada y guarda los datos en un archivo CSV.

### BOT.ipynb

Este notebook contiene la implementación del chatbot que interactúa con el usuario para recopilar información y verificar la cobertura de servicios de seguridad en su área.

### Bot Machine Learning.ipynb

Este notebook implementa algoritmos de aprendizaje automático para mejorar la funcionalidad del chatbot, incluyendo la predicción de la cobertura y la clasificación de los códigos postales en función de los datos proporcionados.