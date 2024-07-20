
# Lib Admin

Lib Admin, es un Sistema de Gestión de Bibliotecas utilizando una base de datos MySQL. Ya sea que estés administrando una pequeña biblioteca personal o una colección institucional más grande, este sistema proporciona una forma simple de llevar un registro de la información y las interacciones de los usuarios con la biblioteca.

## Características

- **Autenticación de usuario:** Permite a los usuarios registrarse e iniciar sesión.
- **Gestión de libros:** Funcionalidades para agregar, buscar y ver detalles de libros.
- **Asignación de libros:** Permite a los usuarios asignar libros y ver cuántos libros están disponibles o prestados.
- **Notificaciones:** Mensajes de éxito o error para las acciones realizadas por los usuarios.

## Tecnologías Utilizadas

- **Flask**: Un framework de aplicaciones web WSGI ligero en Python.
- **MySQL**: Un sistema de gestión de bases de datos relacional para manejar los datos de los usuarios.
- **HTML/CSS**: Para crear la interfaz web.

## Instalación de un Entorno Virtual de Python

Para crear y activar un entorno virtual en Python, sigue los siguientes pasos:

### Paso 1: Instalación de `venv`

Python 3 incluye el módulo `venv` por defecto. Si estás usando Python 3.3 o superior, no necesitas instalar nada adicional. Simplemente asegúrate de tener Python 3 instalado en tu sistema. Puedes verificar esto ejecutando:

```sh
python3 --version
```

### Paso 2: Crear un Entorno Virtual

Navega hasta el directorio de tu proyecto y crea un entorno virtual ejecutando el siguiente comando:

```sh
python3 -m venv nombre_del_entorno
```

Reemplaza `nombre_del_entorno` con el nombre que quieras darle a tu entorno virtual.

### Paso 3: Activar el Entorno Virtual

Después de crear el entorno virtual, debes activarlo. El comando para activar el entorno virtual varía según el sistema operativo que estés utilizando.

- **En Windows**:

  ```sh
  .\nombre_del_entorno\Scripts\activate
  ```

- **En macOS y Linux**:

  ```sh
  source nombre_del_entorno/bin/activate
  ```

### Paso 4: Verificar que el Entorno Virtual está Activado

Cuando el entorno virtual esté activado, deberías ver el nombre del entorno en el prompt de tu terminal, algo como esto:

```sh
(nombre_del_entorno) $
```

### Paso 5: Instalar Dependencias

Con el entorno virtual activado, puedes instalar las dependencias de tu proyecto. Por ejemplo, para instalar las dependencias listadas en un archivo `requirements.txt`, usa:

```sh
pip install -r requirements.txt
```

### Paso 6: Desactivar el Entorno Virtual

Para desactivar el entorno virtual y volver al entorno global de Python, simplemente ejecuta:

```sh
deactivate
```

## Instalación

Para obtener una copia local y ponerla en funcionamiento, sigue estos simples pasos:

1. **Clona el repositorio**
   ```sh
   git clone https://github.com/cdavidbm/libadmin.git
   ```
2. **Instala las dependencias**
   ```sh
   pip install -r requirements.txt
   ```
   Contenido del archivo `requirements.txt`:
   ```
   flask==2.3.2
   flask-mysql==1.5.2
   timeago==1.0.15
   ```
3. **Configura la base de datos**
   - Asegúrate de que MySQL esté instalado y en funcionamiento.
   - Crea una base de datos y actualiza la configuración de la base de datos en el archivo `config.py`.

4. **Ejecuta la aplicación**
   ```sh
   flask run
   ```

## Uso

Una vez que la aplicación esté en funcionamiento, puedes acceder a ella en tu navegador web en `http://127.0.0.1:5000`. Desde allí, puedes comenzar a gestionar los usuarios de la biblioteca navegando a través de la interfaz proporcionada.

## Contribuciones

Las contribuciones son lo que hace que la comunidad de código abierto sea un lugar increíble para aprender, inspirar y crear. Cualquier contribución que hagas es **muy apreciada**.

1. Haz un fork del proyecto.
2. Crea tu rama de características (`git checkout -b feature/AmazingFeature`).
3. Realiza tus cambios (`git commit -m 'Add some AmazingFeature'`).
4. Empuja a la rama (`git push origin feature/AmazingFeature`).
5. Abre un Pull Request.

## Licencia

Distribuido bajo la Licencia MIT. Consulta el archivo `LICENSE` para más información.
