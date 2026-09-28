# 🏥 Sistema de Gestión de Citas Médicas

> Aplicación web desarrollada con **Django** para centralizar la gestión de pacientes, médicos, citas y procesos relacionados con la atención médica.

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python\&logoColor=white)
![Django](https://img.shields.io/badge/Django-Web%20Framework-green?logo=django\&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-UI-7952B3?logo=bootstrap\&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Frontend-yellow?logo=javascript\&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database-336791?logo=postgresql\&logoColor=white)

---

## ✨ Sobre el proyecto

El **Sistema de Gestión de Citas Médicas** es una aplicación web diseñada para organizar y centralizar diferentes procesos relacionados con la atención médica.

El sistema permite gestionar información de **pacientes, médicos, citas, atenciones médicas, medicamentos y exámenes**, incorporando además autenticación de usuarios, control de permisos, generación de documentos y comunicación mediante correo electrónico.

El proyecto busca reducir la dependencia de procesos manuales y facilitar el acceso organizado a la información desde una plataforma web.

---

## 🎯 Problema que aborda

La gestión manual de citas e información médica puede generar problemas como:

* Dificultad para organizar las citas.
* Información distribuida en diferentes medios.
* Complicaciones para consultar registros de pacientes.
* Falta de seguimiento de las atenciones.
* Acceso no controlado a determinada información.
* Mayor trabajo administrativo.

### 💡 Solución

La aplicación centraliza estos procesos en una plataforma web donde los usuarios pueden gestionar la información de acuerdo con sus permisos y consultar los datos necesarios para llevar un mejor control de la atención médica.

---

## 🚀 Funcionalidades principales

### 👤 Autenticación y usuarios

* Registro de usuarios.
* Inicio y cierre de sesión.
* Gestión de perfiles.
* Control de acceso mediante permisos.
* Diferenciación de funcionalidades según el tipo de usuario.

### 🧑‍⚕️ Gestión médica

* Registro y gestión de médicos.
* Registro y gestión de pacientes.
* Administración de información relacionada con los pacientes.
* Gestión de tipos de sangre.

### 📅 Gestión de citas

* Creación de citas médicas.
* Consulta de citas.
* Visualización de próximas citas.
* Seguimiento de la atención asociada a cada cita.

### 🩺 Atenciones médicas

El sistema permite registrar información relacionada con las atenciones realizadas, manteniendo un seguimiento de los procesos médicos asociados al paciente.

### 💊 Medicamentos

* Registro de medicamentos.
* Gestión de información relacionada con tratamientos.
* Asociación de medicamentos con las atenciones correspondientes.

### 🧪 Exámenes

* Registro de exámenes solicitados.
* Gestión de información relacionada con los exámenes.
* Asociación con la atención médica correspondiente.

### 📄 Documentos

* Generación de documentos en formato PDF.
* Preparación de información para ser consultada o compartida.

### 📧 Comunicación

El sistema incorpora envío de correos electrónicos mediante **Resend**, permitiendo automatizar determinadas comunicaciones de la aplicación.

### 💳 Pagos

Se incorporó integración con **PayPal** para permitir el manejo de procesos de pago dentro de la aplicación.

---

## 🖥️ Interfaz

La aplicación utiliza **Bootstrap, HTML, CSS y JavaScript** para construir una interfaz web organizada y adaptable.

> 📸 *Puedes colocar aquí capturas de pantalla de las principales páginas del sistema.*

Algunas capturas que quedarían bien en el README:

* 🔐 Inicio de sesión
* 🏠 Dashboard
* 📅 Gestión de citas
* 👨‍⚕️ Gestión de médicos
* 🧑‍🤝‍🧑 Gestión de pacientes
* 🩺 Registro de atención
* 📊 Actividad reciente

---

## 🛠️ Tecnologías utilizadas

| Tecnología                  | Uso                                              |
| --------------------------- | ------------------------------------------------ |
| 🐍 **Python**               | Lenguaje principal                               |
| 🌐 **Django**               | Desarrollo del backend y lógica de la aplicación |
| 🖥️ **HTML / CSS**          | Estructura y estilos                             |
| 🎨 **Bootstrap**            | Diseño de la interfaz                            |
| ⚡ **JavaScript**            | Interactividad del frontend                      |
| 🗄️ **SQLite**              | Base de datos para desarrollo                    |
| 🐘 **PostgreSQL**           | Base de datos relacional                         |
| 📄 **ReportLab**            | Generación de documentos PDF                     |
| 🖼️ **Pillow**              | Procesamiento de imágenes                        |
| 🧩 **django-widget-tweaks** | Personalización de formularios                   |
| 🔧 **django-extensions**    | Herramientas adicionales para Django             |
| ⏰ **django-celery-beat**    | Programación de tareas                           |
| 📧 **Resend**               | Envío de correos electrónicos                    |
| 💳 **PayPal REST SDK**      | Integración de pagos                             |
| 🔐 **python-dotenv**        | Gestión de variables de entorno                  |

---

## 🧱 Arquitectura general

El proyecto está organizado siguiendo la estructura de un proyecto Django, separando las aplicaciones, recursos estáticos, plantillas y archivos de configuración.

```text
Citas-Medicas/
│
├── 📁 aplication/
│   └── Lógica y funcionalidades principales
│
├── 📁 doctor/
│   └── Funcionalidades relacionadas con el área médica
│
├── 📁 static/
│   └── Archivos estáticos
│
├── 📁 template/
│   └── Plantillas HTML
│
├── 📁 media/
│   └── Archivos multimedia
│
├── manage.py
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

---

## 🔐 Seguridad y configuración

El proyecto utiliza variables de entorno para evitar almacenar directamente información sensible dentro del código fuente.

Se proporciona un archivo:

```text
.env.example
```

como referencia para configurar las variables necesarias.

> ⚠️ Las credenciales, claves API y demás información sensible no deben almacenarse directamente en el repositorio.

---

## ⚙️ Instalación

### 1. Clonar el repositorio

```bash
git clone https://github.com/TU-USUARIO/Citas-Medicas.git
```

### 2. Entrar al proyecto

```bash
cd Citas-Medicas
```

### 3. Crear un entorno virtual

```bash
python -m venv venv
```

Activarlo en Windows:

```bash
venv\Scripts\activate
```

En Linux/macOS:

```bash
source venv/bin/activate
```

### 4. Instalar las dependencias

```bash
pip install -r requirements.txt
```

### 5. Configurar las variables de entorno

Crear un archivo `.env` tomando como referencia:

```text
.env.example
```

### 6. Ejecutar las migraciones

```bash
python manage.py migrate
```

### 7. Ejecutar el servidor

```bash
python manage.py runserver
```

La aplicación estará disponible localmente en:

```text
http://127.0.0.1:8000/
```

---

## 📚 Lo que trabajé en este proyecto

Este proyecto permitió aplicar conocimientos de **desarrollo web, bases de datos y construcción de aplicaciones con Django**, trabajando aspectos como:

* Desarrollo de aplicaciones web con Python y Django.
* Diseño y organización de módulos.
* Gestión de usuarios y autenticación.
* Control de permisos y acceso.
* Manejo de formularios.
* Persistencia de información en bases de datos.
* Integración entre backend y frontend.
* Generación de documentos PDF.
* Envío de correos electrónicos.
* Integración con servicios externos mediante APIs.
* Manejo de variables de entorno.
* Organización de un proyecto mediante una estructura modular.

---

## 🔮 Posibles mejoras

Algunas funcionalidades que podrían incorporarse en futuras versiones:

* [ ] Panel administrativo con estadísticas.
* [ ] Calendario interactivo para médicos y pacientes.
* [ ] Recordatorios automáticos de citas.
* [ ] Historial médico más completo.
* [ ] Notificaciones en tiempo real.
* [ ] Sistema de búsqueda y filtros avanzados.
* [ ] Mejoras de accesibilidad.
* [ ] Pruebas automatizadas.
* [ ] Despliegue en un entorno de producción.
* [ ] Aplicación móvil complementaria.

---

## 🎓 Contexto académico

Proyecto desarrollado como parte del proceso de aprendizaje en **Ingeniería de Software**, aplicando conocimientos de programación, desarrollo web, bases de datos y construcción de software.

---

## 👩‍💻 Autora

**Dyanne**

Estudiante de **Ingeniería de Software**, interesada en el desarrollo de aplicaciones web, resolución de problemas y aprendizaje de nuevas tecnologías.

---

⭐ Si encuentras interesante el proyecto, puedes darle una estrella al repositorio.
