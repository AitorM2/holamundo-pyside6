# Hola mundo con PySide6

En este repositorio vamos a ver como hacer un "Hola mundo" utilizando **PySide6**. Mostrando la instalación y configuracion para Windows
## Requisitos:

- Python 3 (Versión 3.8 o superior).
- pip (administrador de paquetes de Python).

## Instalación y Configuración del entorno

1. **Instalación de python.**
- Descarga python desde la página web -> [Python](https://www.python.org/downloads/).
- Cuando sigas los pasos en el instalador asegurate de marcar la opción `Add Python to PATH`.

2. **Verifica la instalación de python y de pip usando los siguientes comandos.**
```sh
   python --version
   pip --version
```
3. **Creación y activación de un entorno virtual usando los siguientes comandos.**
```sh
   python -m venv nombre_que_le_quieras_dar
   nombre_que_le_quieras_dar\Scripts\activate
```
4. **Instalación de la dependencia Pyside6 usando el siguiente comando.**
 ```sh
   pip install PySide6
 ```
5. **Para ejecutar el programa usaremos el siguiente código.**
 ```sh
   python main.py
 ```

## A continuación proporciono un código de ejemplo que guardaremos en un archivo python llamandolo `main.py`

```python
import sys
from PySide6.QtWidgets import QApplication, QLabel

app = QApplication(sys.argv)
label = QLabel("¡Hola, Mundo!")
label.show()
sys.exit(app.exec())
```
