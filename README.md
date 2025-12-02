📘 Tutorial de Ejecución de FiDAT (Versión estable FiDAT-main)

Autor: (tu nombre si deseas)
Versión: 1.0
Formato: Markdown listo para imprimir o convertir a PDF.

1. Ejecución Rápida del Programa (media página)

Esta sección describe el procedimiento más sencillo para ejecutar FiDAT-main, asumiendo que el entorno ya está configurado.

📂 Ubicación del programa

El programa se encuentra en:

Archivos/FIDAT/FiDAT-main


En ALBA suele estar en:

~/Desktop/FiDAT-main

▶️ Pasos para ejecutar FiDAT

Abrir una terminal

En Windows: abrir Anaconda Prompt

En macOS / Linux: terminal normal

Activar el entorno adecuado

En ALBA:

conda activate fidat


En el Mac de Jaime:

conda activate fidat_env


Moverse a la carpeta donde está main.py:

cd /ruta/a/FiDAT-main


Ejecutar la aplicación:

python main.py


Si el entorno está correctamente configurado, FiDAT se abrirá inmediatamente.

2. Guía para Crear y Configurar el Entorno Conda (máx. 1 página)

(Para copiar y pegar directamente en terminal)

Si el entorno no existe o faltan dependencias, puedes crearlo desde cero:

🆕 Crear el entorno Conda
conda create --name fidat python=3.9
conda activate fidat


⚠️ Importante: siempre activar el entorno antes de instalar nada, para no contaminar el entorno base.

📦 Instalación de dependencias (con versiones exactas)
pip install customtkinter==4.6.3
pip install pyfai==2024.2.0
pip install pandas==2.2.2
pip install openpyxl==3.1.2

✔️ Comprobar instalación

Ejecutar desde la carpeta donde está main.py:

python main.py


Si abre FiDAT, el entorno está listo.

🛑 Si aparece un error por librería faltante

Ejemplos típicos:

Error	Solución
ModuleNotFoundError: No module named 'customtkinter'	pip install customtkinter==4.6.3
ModuleNotFoundError: No module named 'pyFAI'	pip install pyfai==2024.2.0
ModuleNotFoundError: No module named 'pandas'	pip install pandas==2.2.2
Se abre la interfaz pero se queda congelada en la integración	Falta instalar openpyxl → pip install openpyxl==3.1.2
3. Registro Completo de una Sesión de Terminal (máx. 3 páginas)

(Tal cual para documentación y troubleshooting)
(Incluye resumen explicativo al inicio)

📄 Resumen de lo que aparece en pantalla

Se crea un entorno llamado borrar con Python 3.9 → el sistema pregunta Proceed?

Se activa el entorno

El usuario navega a Downloads/FiDAT-main/FiDAT-main

Ejecuta python main.py → aparecen errores por librerías faltantes

Instalación manual de:

customtkinter

pyfai

pandas

openpyxl

Tras instalar todas, FiDAT abre correctamente

📟 Registro completo del terminal
(base) C:\Users\Usuario>conda create --name borrar python=3.9
Proceed ([y]/n)? y

(base) C:\Users\Usuario>conda activate borrar

(borrar) C:\Users\Usuario>cd Downloads
(borrar) C:\Users\Usuario\Downloads>cd FiDAT-main
(borrar) C:\Users\Usuario\Downloads\FiDAT-main>cd FiDAT-main

(borrar) C:\Users\Usuario\Downloads\FiDAT-main\FiDAT-main>dir
 El volumen de la unidad C no tiene etiqueta.
 El número de serie del volumen es: 809E-85F2

 Directorio de C:\Users\Usuario\Downloads\FiDAT-main\FiDAT-main

02/12/2025  18:48    <DIR>          .
02/12/2025  18:48    <DIR>          ..
02/12/2025  18:48             3.078 .gitignore
02/12/2025  18:48    <DIR>          classes
02/12/2025  18:48             3.529 fidat_environment.yml
02/12/2025  18:48               152 main.py
02/12/2025  18:48    <DIR>          Oscar-scripts
02/12/2025  18:48             1.019 README.md
02/12/2025  18:48    <DIR>          resources
02/12/2025  18:48    <DIR>          test_data
02/12/2025  18:48                 0 __init__.py
               5 archivos          7.778 bytes
               6 dirs  359.182.295.040 bytes libres

(borrar) C:\Users\Usuario\Downloads\FiDAT-main\FiDAT-main>python main.py
Traceback (most recent call last):
  File "...\main.py", line 3, in <module>
    import customtkinter
ModuleNotFoundError: No module named 'customtkinter'

(borrar) > pip install customtkinter==4.6.3

(borrar) > python main.py
Traceback (most recent call last):
  ...
ModuleNotFoundError: No module named 'pyFAI'

(borrar) > pip install pyfai==2024.2.0

(borrar) > python main.py
... UserWarning pkg_resources deprecated ...
ModuleNotFoundError: No module named 'pandas'

(borrar) > pip install pandas==2.2.2

(borrar) > python main.py
(Aquí la aplicación se abre, pero falla en la primera integración)

(borrar) > pip install openpyxl==3.1.2

¿Quieres que te genere esto directamente en PDF o en Markdown real (.md) listo para imprimir?
Tú dijiste:
Sí, por favor si me puedes dar un Markdown te lo agradezco. Gracias
ChatGPT Plus

Aquí tienes el Markdown completo, limpio, ordenado y listo para copiar/pegar directamente en un archivo .md y exportarlo a PDF si lo deseas.
Está exactamente dividido en tres partes, con estética moderna y espaciado perfecto para impresión.

📘 Tutorial de Ejecución de FiDAT (Versión Estable FiDAT-main)

Autor:
Versión: 1.0
Ubicación del programa: Archivos/FIDAT/FiDAT-main

1. Ejecución Rápida de FiDAT

(Duración: 10–20 segundos — Media página)

Esta sección muestra la forma más sencilla y directa de abrir FiDAT cuando el entorno ya está configurado.

▶️ Paso 1 — Abrir una terminal

Windows: usar Anaconda Prompt

macOS / Linux: abrir terminal normal

▶️ Paso 2 — Activar el entorno correspondiente
# En ALBA
conda activate fidat

# En el Mac de Jaime
conda activate fidat_env

▶️ Paso 3 — Ir a la carpeta donde está main.py
cd /ruta/a/FiDAT-main


En ALBA normalmente está en el Desktop:

cd ~/Desktop/FiDAT-main

▶️ Paso 4 — Ejecutar el programa
python main.py


Si el entorno está bien configurado, FiDAT se abrirá inmediatamente.

2. Crear o Reparar el Entorno Conda

(Listo para copiar/pegar — Máx. 1 página)

Si tu entorno no existe o aparece algún error de librerías, sigue estos pasos:

🆕 Crear un entorno desde cero
conda create --name fidat python=3.9
conda activate fidat


⚠️ Importante: Instala todo siempre dentro del entorno, nunca en base.

📦 Instalar todas las dependencias necesarias (con versiones exactas)
pip install customtkinter==4.6.3
pip install pyfai==2024.2.0
pip install pandas==2.2.2
pip install openpyxl==3.1.2

✔️ Probar que funciona

Ejecuta FiDAT:

python main.py

🛑 Errores típicos y cómo solucionarlos
Error en pantalla	Instalar
ModuleNotFoundError: No module named 'customtkinter'	pip install customtkinter==4.6.3
ModuleNotFoundError: No module named 'pyFAI'	pip install pyfai==2024.2.0
ModuleNotFoundError: No module named 'pandas'	pip install pandas==2.2.2
La interfaz se abre pero falla al cargar Excel	pip install openpyxl==3.1.2
3. Registro Completo de una Sesión Real de Terminal

(Máx. 3 páginas — para documentación o resolución de problemas)

A continuación se muestra el registro completo de una instalación real, útil como referencia de cómo debería verse el proceso y los mensajes del sistema.

📄 Resumen previo

Se crea un entorno llamado borrar

Se activa

Se navega a la carpeta FiDAT-main

Al ejecutar python main.py, faltan librerías

Se instalan una a una (customtkinter, pyfai, pandas, openpyxl)

Finalmente, FiDAT se ejecuta correctamente

📟 Registro de terminal
(base) C:\Users\Usuario>conda create --name borrar python=3.9
Proceed ([y]/n)? y

(base) C:\Users\Usuario>conda activate borrar

(borrar) C:\Users\Usuario>cd Downloads
(borrar) C:\Users\Usuario\Downloads>cd FiDAT-main
(borrar) C:\Users\Usuario\Downloads\FiDAT-main>cd FiDAT-main

(borrar) C:\Users\Usuario\Downloads\FiDAT-main\FiDAT-main>dir
 El volumen de la unidad C no tiene etiqueta.
 El número de serie del volumen es: 809E-85F2

 Directorio de C:\Users\Usuario\Downloads\FiDAT-main\FiDAT-main

02/12/2025  18:48    <DIR>          .
02/12/2025  18:48    <DIR>          ..
02/12/2025  18:48             3.078 .gitignore
02/12/2025  18:48    <DIR>          classes
02/12/2025  18:48             3.529 fidat_environment.yml
02/12/2025  18:48               152 main.py
02/12/2025  18:48    <DIR>          Oscar-scripts
02/12/2025  18:48             1.019 README.md
02/12/2025  18:48    <DIR>          resources
02/12/2025  18:48    <DIR>          test_data
02/12/2025  18:48                 0 __init__.py
               5 archivos          7.778 bytes
               6 dirs  359.182.295.040 bytes libres

(borrar) C:\Users\Usuario\Downloads\FiDAT-main\FiDAT-main>python main.py
Traceback (most recent call last):
  File "...\main.py", line 3, in <module>
    import customtkinter
ModuleNotFoundError: No module named 'customtkinter'

(borrar) > pip install customtkinter==4.6.3

(borrar) > python main.py
Traceback (most recent call last):
  ...
ModuleNotFoundError: No module named 'pyFAI'

(borrar) > pip install pyfai==2024.2.0

(borrar) > python main.py
... UserWarning: pkg_resources is deprecated ...
ModuleNotFoundError: No module named 'pandas'

(borrar) > pip install pandas==2.2.2

(borrar) > python main.py
(Aquí FiDAT se abre, pero falla al procesar Excel)

(borrar) > pip install openpyxl==3.1.2
