Cookiecutter Personal
Aprende a crear tu propia plantilla personalizada utilizando Cookiecutter.

Requerimientos
Anaconda >= 4.x
Git >= 2.x
Cookiecutter Python package >= 1.4.0. Esto puede ser instalado con pip o conda dependiendo de cómo manejas tus paquetes de Python:

pip install cookiecutter
o
conda install -c conda-forge cookiecutter

Crear un nuevo proyecto
En el directorio donde deseas guardar tu proyecto generado:

cookiecutter https://github.com/nicolascard995/Template Data science 1 --checkout cookiecutter-personal

Estructura de directorios y archivos resultantes
{{ cookiecutter.project_slug }}
    ├── data
    │   ├── processed      <- Los conjuntos de datos finales y canónicos para el modelado.
    │   └── raw            <- La copia de seguridad original e inmutable de los datos.
    │
    ├── notebooks          <- Notebooks de Jupyter. La convención de nomenclatura es un número (para ordenar), las iniciales del creador y una breve descripción separada por guiones, por ejemplo, `1.0-jvelez-inicio-exploracion-datos`.
    │
    ├── .gitignore         <- Archivos ignorados por `git`.
    │
    ├── environment.yml    <- Archivo de requisitos para reproducir el ambiente de análisis.
    │
    └── README.md          <- El README de nivel superior para los desarrolladores que utilizan este proyecto.

Plantilla creada por {{ Nicolás Alejandro Cardozo }}.

lisences