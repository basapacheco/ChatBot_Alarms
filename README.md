# ChatBot_Alarms

`ChatBot_Alarms` es un proyecto que consiste en un chatbot diseñado para ayudar a los usuarios a verificar la cobertura de seguridad en sus códigos postales y proporcionar información sobre los servicios de alarma. El proyecto se compone de varias partes, incluidas carpetas de datos, scripts en Jupyter Notebook y archivos CSV para el manejo de la información.

## Estructura del Proyecto

- `codigos1220n/`: Carpeta que contiene 152 archivos .txt con todos los códigos postales y los barrios correspondientes de España.
- `BOT.ipynb`: Jupyter Notebook que implementa la lógica principal del chatbot.
- `Bot Machine Learning.ipynb`: Jupyter Notebook para implementar algoritmos de aprendizaje automático relacionados con el chatbot.
- `CP_generator.ipynb`: Jupyter Notebook que genera un archivo CSV con los códigos postales y su cobertura.
- `Bot_IA.ipynb`: Jupyter Notebook que integra capacidades de inteligencia artificial (IA) para mejorar la interacción del chatbot con los usuarios.
- `cobertura.csv`: Archivo CSV que contiene la cobertura de los códigos postales.
- `registros.csv`: Archivo CSV que almacena los datos de los usuarios que interactúan con el chatbot.

## Descripción de los Jupyter Notebooks

### CP_generator.ipynb

Este script lee los archivos de texto en la carpeta `codigos1220n` y extrae los códigos postales y localidades. Luego, genera una cobertura aleatoria para cada entrada y guarda los datos en un archivo CSV.

### BOT.ipynb

Este notebook contiene la implementación del chatbot que interactúa con el usuario para recopilar información y verificar la cobertura de servicios de seguridad en su área. Utiliza reglas predefinidas y manejo de excepciones para asegurar una interacción fluida.

### Bot Machine Learning.ipynb

Este notebook implementa algoritmos de aprendizaje automático para mejorar la funcionalidad del chatbot, incluyendo la predicción de la cobertura y la clasificación de los códigos postales en función de los datos proporcionados.

### Bot_IA.ipynb

Este notebook integra capacidades de inteligencia artificial utilizando el modelo `gpt-2` de Hugging Face para generar respuestas más naturales y contextuales. Incluye:

- **Hugging Face Pipeline**: Utiliza la función `pipeline` de Hugging Face para cargar el modelo `gpt-2`.
- **Normalización de la Entrada**: Asegura que las entradas del usuario sean entendidas de manera consistente, independientemente de mayúsculas, minúsculas o errores tipográficos comunes.
- **Manejo de Excepciones**: Agrega manejo de excepciones para robustez y seguridad.
- **Ejecución de Notebooks**: Ejecuta el notebook `CP_generator.ipynb` si el archivo `cobertura.csv` no está presente.

## Cómo Empezar

Para ejecutar este proyecto, sigue estos pasos:

1. **Clona el repositorio**:
    ```sh
    git clone https://github.com/basapacheco/ChatBot_Alarms.git
    cd ChatBot_Alarms
    ```

2. **Instala las dependencias**:
    Asegúrate de tener `pip` y `conda` instalados. Luego, ejecuta:
    ```sh
    pip install -r requirements.txt
    ```

3. **Ejecuta los notebooks**:
    Abre Jupyter Notebook y ejecuta los notebooks en el siguiente orden:
    - `CP_generator.ipynb`
    - `Bot_IA.ipynb` (o `BOT.ipynb` y `Bot Machine Learning.ipynb` si prefieres la versión sin IA)

4. **Interacción con el chatbot**:
    Sigue las instrucciones del chatbot en el notebook para proporcionar información y recibir retroalimentación sobre la cobertura y servicios de seguridad.

## Contribuciones

Las contribuciones son bienvenidas. Por favor, abre un issue o un pull request para discutir cualquier cambio o mejora.

## Licencia

Este proyecto está licenciado bajo los términos de la licencia MIT. Consulta el archivo LICENSE para más detalles.
