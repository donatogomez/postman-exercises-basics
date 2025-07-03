# 🧪 Postman Exercises · Fundamentals for API Testing

Repositorio técnico con una serie de ejercicios básicos e intermedios para practicar el uso de Postman. Este material está pensado como recurso didáctico y profesional, enfocado a desarrolladores backend o mobile que trabajan integrando APIs REST. Aquí se documenta el uso correcto de entornos, variables, scripting, validación de respuestas y ejecución automatizada.

> 📌 Ideal para reforzar conocimientos de testing de endpoints, preparación de datos y flujos de CI, o como base para mentoring técnico.

---

## 📚 Índice de ejercicios

| Nº | Ejercicio                          | Descripción técnica                                                 |
|----|------------------------------------|----------------------------------------------------------------------|
| 1  | [GET Request](docs/01_GET_request.md)              | Consulta básica con verificación de status y estructura del JSON     |
| 2  | [POST Request](docs/02_POST_request.md)            | Envío de payload JSON con validación del response                    |
| 3  | [Variables en entorno](docs/03_variables_env.md)   | Parametrización de URLs y datos dinámicos usando entorno local       |
| 4  | [Colecciones](docs/04_collections.md)              | Agrupación de peticiones y estructuración para pruebas               |
| 5  | [Pre-request Scripts](docs/05_pre_request_scripts.md) | Generación dinámica de datos antes del envío de la petición          |
| 6  | [Tests en respuestas](docs/06_tests.md)            | Validación automática de claves en JSON y códigos de estado          |
| 7  | [Runner & Automatización](docs/07_runner.md)       | Ejecución por lotes con múltiples iteraciones                        |

---

## 🧩 Estructura del repositorio

```plaintext
postman-exercises-basics/
├── README.md                    # Documentación general del repo
├── LICENSE                      # Licencia MIT
├── .gitignore                   # Archivos ignorados por Git
│
├── collections/                 # Colecciones Postman en formato JSON
│   └── My_first_collection.postman_collection.json
│
├── environments/                # Entornos exportables (.postman_environment.json)
│   └── local_environment.json
│
├── docs/                        # Documentación por ejercicio (Markdown)
│   ├── 01_GET_request.md
│   ├── 02_POST_request.md
│   └── …
│
├── screenshots/                 # Capturas de pantalla por paso/prueba
│   ├── 01_get_request.png
│   ├── 02_post_request.png
│   └── …
│
└── runner-reports/              # Evidencias de ejecución en batch
└── runner_result_5_iterations.png
```

---

## 🧪 Cómo trabajar con este repositorio


1. Clona el repositorio:
```bash
git clone https://github.com/tu-usuario/postman-exercises-basics.git
cd postman-exercises-basics
```  
2.	Abre Postman:
    - Importa la colección desde collections/
    - Importa el entorno desde environments/  
3.	Sigue los pasos descritos en cada fichero dentro de docs/.  
4.	Comprueba el resultado de cada ejercicio en screenshots/.  
5.	Ejecuta tests en lote desde el Runner e incluye las capturas generadas en runner-reports/.

---

## 🧠 Objetivo del repositorio

 Este proyecto sirve como punto de partida para:
 - Formación técnica en equipos mobile/backend
 - Mentorización en prácticas de testing y automatización
 - Documentación de buenas prácticas para proyectos reales
 - Preparación de CI pipelines orientados a integración de APIs

---

## 📚 Recursos recomendados

- Postman Learning Center
- Postman Scripting Docs (JavaScript)
- Public APIs para pruebas

---

## 🪪 Licencia

Distribuido bajo licencia MIT.  
Uso libre con atribución.
