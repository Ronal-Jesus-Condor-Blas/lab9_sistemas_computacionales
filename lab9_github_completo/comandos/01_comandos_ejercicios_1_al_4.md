# Comandos utilizados en los ejercicios 1 al 4

## Ejercicio 1: Navegación del sistema de archivos y creación de directorios

```bash
pwd
cd /
pwd
cd ~
mkdir -p practica_linux/laboratorio/archivos
cd practica_linux/laboratorio/archivos
```

### Explicación

- `pwd`: muestra la ruta absoluta del directorio actual.
- `cd /`: cambia al directorio raíz del sistema Linux.
- `cd ~`: retorna al directorio personal del usuario.
- `mkdir -p practica_linux/laboratorio/archivos`: crea una estructura de carpetas anidadas. La opción `-p` permite crear también los directorios padres si no existen.
- `cd practica_linux/laboratorio/archivos`: ingresa al directorio `archivos` usando una ruta relativa.

---

## Ejercicio 2: Creación, redirección y lectura de archivos

```bash
echo "Sistemas Computacionales" > sistema.txt
echo "Tercer Semestre" > semestre.txt
cat sistema.txt semestre.txt > resumen.txt
less resumen.txt
mv resumen.txt .resumen.txt
ls
ls -a
```

### Explicación

- `echo "Sistemas Computacionales" > sistema.txt`: crea el archivo `sistema.txt` con el texto indicado.
- `echo "Tercer Semestre" > semestre.txt`: crea el archivo `semestre.txt` con el texto indicado.
- `cat sistema.txt semestre.txt > resumen.txt`: une el contenido de ambos archivos y lo guarda en `resumen.txt`.
- `less resumen.txt`: permite visualizar el contenido del archivo por páginas.
- `mv resumen.txt .resumen.txt`: renombra el archivo agregando un punto al inicio para convertirlo en oculto.
- `ls`: lista archivos visibles.
- `ls -a`: lista todos los archivos, incluyendo archivos ocultos.

---

## Ejercicio 3: Acceso a archivos y privilegios administrativos

```bash
cat /etc/shadow
sudo cat /etc/shadow
echo "El uso de sudo limita el tiempo de exposición de privilegios administrativos, restringe las acciones según el usuario y evita errores accidentales que podrían ocurrir si se mantiene una sesión permanente como root." >> seguridad.txt
```

### Explicación

- `cat /etc/shadow`: intenta leer un archivo protegido del sistema. Sin privilegios administrativos, el acceso es denegado.
- `sudo cat /etc/shadow`: ejecuta el comando con privilegios administrativos temporales.
- `echo ... >> seguridad.txt`: agrega una justificación teórica al archivo `seguridad.txt`. El operador `>>` añade contenido sin reemplazar lo existente.

---

## Ejercicio 4: Automatización mediante scripts

```bash
cd ~/practica_linux
nano info_entorno.sh
chmod +x info_entorno.sh
./info_entorno.sh
```

Contenido del script:

```bash
#!/bin/bash
echo "Directorio de trabajo actual:"
pwd
echo "Listado detallado del contenido del directorio:"
ls -la
```

### Explicación

- `cd ~/practica_linux`: ingresa al directorio principal de trabajo.
- `nano info_entorno.sh`: crea o edita el archivo del script desde consola.
- `chmod +x info_entorno.sh`: otorga permiso de ejecución al script.
- `./info_entorno.sh`: ejecuta el script usando la ruta relativa actual.
- `pwd`: dentro del script, muestra el directorio actual.
- `ls -la`: dentro del script, muestra el contenido detallado del directorio, incluyendo archivos ocultos y permisos.
