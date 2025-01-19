# **Módulo 2: Manejo de Archivos y Estructura del Sistema**

## **Gestión de Archivos y Directorios**

### **Comandos básicos:**

-   **Copiar archivos o directorios:**
    ```bash
    cp [origen] [destino]
    ```
-   **Mover archivos o directorios:**
    ```bash
    mv [origen] [destino]
    ```
-   **Eliminar archivos o directorios:**
    ```bash
    rm [archivo_o_directorio]
    ```
-   **Crear un directorio:**
    ```bash
    mkdir [nombre_del_directorio]
    ```
-   **Crear un archivo vacío:**
    ```bash
    touch [nombre_del_archivo]
    ```

### **Visualización de contenido:**

-   Ver el contenido completo de un archivo:
    ```bash
    cat archivo
    ```
-   Ver las primeras líneas de un archivo:
    ```bash
    head archivo
    ```
-   Ver las últimas líneas de un archivo:
    ```bash
    tail archivo
    ```

---

## **Compresión y Empaquetado**

### **Comandos para empaquetar y comprimir:**

-   Crear un archivo `.tar`:
    ```bash
    tar -cvf archivo.tar archivos
    ```
-   Comprimir con gzip:
    ```bash
    gzip archivo
    ```
-   Comprimir con bzip2:
    ```bash
    bzip2 archivo
    ```
-   Descomprimir un archivo `.tar.gz`:
    ```bash
    tar -xzvf archivo.tar.gz
    ```
-   Descomprimir un archivo `.zip`:
    ```bash
    unzip archivo.zip
    ```

---

### **Resumen de Comandos**

| Comando | Descripción                            |
| ------- | -------------------------------------- |
| `cp`    | Copiar archivos o directorios          |
| `mv`    | Mover o renombrar archivos/directorios |
| `rm`    | Eliminar archivos o directorios        |
| `mkdir` | Crear un nuevo directorio              |
| `chmod` | Cambiar permisos de archivos           |
| `chown` | Cambiar propietario de archivos        |
| `tar`   | Crear o extraer archivos empaquetados  |
| `gzip`  | Comprimir archivos                     |
| `unzip` | Descomprimir archivos ZIP              |

---

## **Estructura del Sistema de Archivos**

-   **Directorios principales:**
    -   `/home`: Directorio personal de los usuarios.
    -   `/etc`: Archivos de configuración del sistema.
    -   `/var`: Archivos variables, como logs.
    -   `/usr`: Archivos de usuario, aplicaciones y librerías.
    -   `/tmp`: Archivos temporales.
