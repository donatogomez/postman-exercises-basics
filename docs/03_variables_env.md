# 🟡 Ejercicio 3 – Uso de variables en Postman

> Parametrizar URLs mediante variables de entorno.  
> Este ejercicio permite mantener endpoints reutilizables y desacoplar valores estáticos en peticiones.

---

## 🧩 Endpoint utilizado

**GET** {{baseUrl}}/posts/1  
(baseUrl definido como variable de entorno)

---

## 🛠 Pasos realizados

1. Abrir Postman.
2. Ir a la pestaña **Environments** y crear uno nuevo con el nombre `Local`.
3. Definir una variable:
   - **Variable:** `baseUrl`
   - **Initial value:** `https://jsonplaceholder.typicode.com`
   - **Current value:** `https://jsonplaceholder.typicode.com`
4. Activar el entorno `Local` en la parte superior derecha.
5. Modificar la URL del `GET` anterior:
   - De: `https://jsonplaceholder.typicode.com/posts/1`
   - A: `{{baseUrl}}/posts/1`
6. Ejecutar la petición.

---

### 📸 Captura

![Uso de variable baseUrl](../screenshots/03_variables_env.png)

---

## 🧠 Observaciones técnicas
- Las variables pueden definirse a nivel de entorno, colección o global.
- El uso de `{{baseUrl}}` mejora la reutilización del request en diferentes entornos (producción, staging, etc.).
- Ideal para pipelines de CI, pruebas automatizadas o trabajo colaborativo.
