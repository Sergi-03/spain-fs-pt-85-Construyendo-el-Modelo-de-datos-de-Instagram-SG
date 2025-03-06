# Spain FS PT 85 - Construyendo el Modelo de Datos de Instagram

Este proyecto consiste en diseñar un modelo de datos para una plataforma similar a Instagram. El objetivo es crear una estructura de base de datos relacional que permita almacenar la información de usuarios, publicaciones, comentarios, seguidores, likes y otros elementos clave de la aplicación.

## Características

- **Usuarios**: Información sobre los usuarios de la plataforma, como su nombre, correo electrónico y foto de perfil.
- **Publicaciones**: Registro de las publicaciones realizadas por los usuarios, incluyendo texto, imágenes y fecha.
- **Comentarios**: Comentarios realizados por los usuarios en las publicaciones.
- **Seguidores**: Relación entre los usuarios para gestionar a quién siguen y quién los sigue.
- **Likes**: Registro de los "me gusta" que los usuarios dan a las publicaciones.

## Tecnologías

Este proyecto está desarrollado utilizando las siguientes tecnologías:

- **SQL**: Lenguaje de consulta estructurado utilizado para la gestión de la base de datos.
- **PostgreSQL**: Sistema de gestión de bases de datos relacional (RDBMS) utilizado para almacenar la información.
- **Diagrama ER (Entidad-Relación)**: Representación visual de las entidades y sus relaciones en el sistema, diseñada para reflejar la estructura de datos.

## Estructura del Modelo de Datos

El modelo de datos está basado en las siguientes entidades y relaciones:

- **Usuarios**: Cada usuario tiene un identificador único, nombre, correo electrónico y foto de perfil.
- **Publicaciones**: Las publicaciones están asociadas a un usuario, tienen un identificador único, un texto, una imagen y una fecha de publicación.
- **Comentarios**: Los comentarios están asociados a una publicación y a un usuario, y contienen texto y fecha.
- **Seguidores**: Cada usuario puede seguir a otros usuarios. La relación de seguidores se maneja en una tabla de relaciones.
- **Likes**: Los likes son dados por los usuarios a las publicaciones, y se registran en una tabla de relaciones.

## Uso

### 1. Clona el repositorio
```bash
git clone https://github.com/Sergi-03/spain-fs-pt-85-Construyendo-el-Modelo-de-datos-de-Instagram-SG.git
cd spain-fs-pt-85-Construyendo-el-Modelo-de-datos-de-Instagram-SG
```

### 2. Instala dependencias
```bash
pipenv install
pipenv shell
```

### 3. Crea la base de datos
```bash
flask db init
flask db migrate -m "Initial migration."
flask db upgrade
```

---


## Contacto

Si tienes preguntas o comentarios, no dudes en contactarme en: [ssegarragarcia@gmail.com]
