# Práctica autodidacta - 10 comandos adicionales

Estos comandos se ejecutaron en una carpeta llamada `practica`.

## Preparación

```bash
cd ~
mkdir practica
cd practica
pwd
```

---

## 1. touch

```bash
echo "COMANDO1: touch"
touch archivo_prueba.txt
ls
```

**Descripción:** crea un archivo vacío llamado `archivo_prueba.txt`.

---

## 2. cp

```bash
echo "COMANDO 2: cp"
echo "Contenido de prueba" > archivo_prueba.txt
cp archivo_prueba.txt copia_archivo.txt
ls
```

**Descripción:** copia `archivo_prueba.txt` y crea `copia_archivo.txt`.

---

## 3. head

```bash
echo -e "Linea 1\nLinea 2\nLinea 3\nLinea 4\nLinea 5" > datos.txt
head datos.txt
```

**Descripción:** muestra las primeras líneas del archivo `datos.txt`.

---

## 4. tail

```bash
tail datos.txt
```

**Descripción:** muestra las últimas líneas del archivo `datos.txt`.

---

## 5. wc

```bash
wc datos.txt
```

**Descripción:** cuenta líneas, palabras y caracteres del archivo `datos.txt`.

---

## 6. grep

```bash
grep "Linea 3" datos.txt
```

**Descripción:** busca la línea que contiene `Linea 3` dentro del archivo `datos.txt`.

---

## 7. find

```bash
find . -name "*.txt"
```

**Descripción:** busca archivos con extensión `.txt` dentro del directorio actual.

---

## 8. date

```bash
date
```

**Descripción:** muestra la fecha y hora del sistema.

---

## 9. whoami

```bash
whoami
```

**Descripción:** muestra el usuario activo en la terminal.

---

## 10. uname

```bash
uname -a
```

**Descripción:** muestra información general del sistema operativo, kernel y arquitectura.
