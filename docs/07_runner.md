# ⚫ Ejercicio 7 – Automatización con Runner en Postman

> Ejecutar una colección completa mediante Runner con múltiples iteraciones.  
> Este ejercicio permite validar flujos de prueba automatizados, especialmente útil para pruebas repetitivas o por lotes.

---

## 🧩 Endpoint utilizado

Colección `My first collection` que contiene:
- **GET** {{baseUrl}}/posts/1
- **POST** {{baseUrl}}/posts (con userId dinámico por script)

---

## 🛠 Pasos realizados

1. Ir a la sección **Collections** en Postman.
2. Seleccionar `My first collection`.
3. Pulsar en **Run collection** (icono ▶️).
4. Configurar los parámetros del Runner:
   - Iterations: `5`
   - Delay: opcional
   - Environment: `Local`
5. Pulsar **Run My first collection**.
6. Observar la ejecución de las 5 iteraciones.

---

### 📸 Captura

![Ejecución del Runner con 5 iteraciones](../screenshots/07_runner.png)
![Resultado del Runner – 5 iteraciones](../runner-reports/runner_result_5_iterations.png)

> Esta imagen muestra el resultado completo de la ejecución en lote.  
> Cada iteración representa un request disparado desde la colección, con su propio `Status` y tiempo de respuesta.

---

## 🧠 Observaciones técnicas
- Runner permite automatizar múltiples ejecuciones con diferentes entradas (ideal si se usa CSV o JSON como datos).
- Las variables generadas dinámicamente se evalúan en cada iteración.
- Puede exportarse la colección con entorno y utilizar **Newman** en línea de comandos para integrarlo en flujos de CI/CD.
