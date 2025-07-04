# 🔵 Ejercicio 4 – Agrupar peticiones en una colección
> Organizar y reutilizar peticiones agrupándolas en una colección de Postman.  
> Este ejercicio introduce una estructura modular para escenarios de testing, documentación y ejecución automatizada.

## 🛠 Pasos realizados

1. Abrir Postman.
2. Ir a la sección **Collections** (barra lateral izquierda).
3. Crear una nueva colección llamada: `Postman Exercises – Fundamentals`.
4. Añadir las peticiones de los ejercicios 1 a 6:
   - Ejercicio 1 – GET
   - Ejercicio 2 – POST
   - Ejercicio 3 – GET con variable
   - Ejercicio 5 – POST con pre-request script
   - Ejercicio 6 – GET con tests
5. Guardar la colección ➡️
[collections/postman_collection.json](../collections/postman_collection.json)

### 📸 Captura

![Colección creada en Postman](../screenshots/04_collections.png)

### 🧠 Observaciones técnicas

- Las colecciones permiten **organizar lógicamente las peticiones** y reutilizar configuraciones comunes.
- Pueden exportarse en `.postman_collection.json` para ser **versionadas o compartidas** con el equipo.
- Son la base para la **automatización** de pruebas (con Runner o Newman).
- Agrupar por funcionalidades (GET, POST, etc.) permite escalar el proyecto y mantenerlo comprensible.
