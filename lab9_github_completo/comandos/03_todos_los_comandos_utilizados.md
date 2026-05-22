# Lista completa de comandos utilizados en el laboratorio

## Comandos principales del laboratorio

| Comando | Uso en el laboratorio |
|---|---|
| `pwd` | Mostrar la ruta actual de trabajo. |
| `cd /` | Ir al directorio raíz. |
| `cd ~` | Volver al directorio personal. |
| `cd practica_linux/laboratorio/archivos` | Entrar a una carpeta usando ruta relativa. |
| `mkdir -p practica_linux/laboratorio/archivos` | Crear carpetas anidadas. |
| `echo "texto" > archivo.txt` | Crear o reemplazar contenido de un archivo. |
| `cat archivo1 archivo2 > resumen.txt` | Unir archivos y redirigir la salida. |
| `less resumen.txt` | Visualizar un archivo por páginas. |
| `mv resumen.txt .resumen.txt` | Renombrar un archivo y convertirlo en oculto. |
| `ls` | Listar archivos visibles. |
| `ls -a` | Listar archivos visibles y ocultos. |
| `cat /etc/shadow` | Intentar leer un archivo protegido. |
| `sudo cat /etc/shadow` | Leer un archivo protegido con privilegios administrativos. |
| `echo "texto" >> seguridad.txt` | Agregar contenido al final de un archivo. |
| `nano info_entorno.sh` | Crear o editar un script. |
| `chmod +x info_entorno.sh` | Dar permiso de ejecución al script. |
| `./info_entorno.sh` | Ejecutar el script creado. |
| `ls -la` | Listar contenido detallado, incluyendo archivos ocultos. |

## Comandos adicionales de la práctica autodidacta

| Comando | Uso en la práctica autodidacta |
|---|---|
| `touch archivo_prueba.txt` | Crear un archivo vacío. |
| `cp archivo_prueba.txt copia_archivo.txt` | Copiar un archivo. |
| `head datos.txt` | Mostrar las primeras líneas de un archivo. |
| `tail datos.txt` | Mostrar las últimas líneas de un archivo. |
| `wc datos.txt` | Contar líneas, palabras y caracteres. |
| `grep "Linea 3" datos.txt` | Buscar texto dentro de un archivo. |
| `find . -name "*.txt"` | Buscar archivos por extensión. |
| `date` | Mostrar fecha y hora del sistema. |
| `whoami` | Mostrar el usuario actual. |
| `uname -a` | Mostrar información general del sistema Linux. |
