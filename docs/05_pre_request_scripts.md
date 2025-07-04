# 🟣 Ejercicio 5 – Uso de Pre-request Scripts en Postman
> Ejecutar JavaScript justo antes de enviar la petición, para generar dinámicamente datos o modificar variables.  
> Este ejercicio introduce automatización básica dentro del ciclo de petición-respuesta.

## 🧩 Endpoint utilizado
**POST** {{baseUrl}}/posts  
(userId generado dinámicamente antes del envío)

## 🛠 Pasos realizados

1. Abrir la petición `POST` usada en el ejercicio 2.
2. Ir a la pestaña **Pre-request Script**.
3. Pegar el siguiente código JavaScript:

```javascript
pm.globals.set("userId", Math.floor(Math.random() * 100));
```
4.	Modificar el body para usar la variable {{userId}}:
```json
{
  "title": "New post",
  "body": "This is the content",
  "userId": {{userId}}
}
```
5.	Pulsar Send varias veces y observar cómo cambia userId dinámicamente.

### 📸 Captura
![Pre-request Script en acción](../screenshots/05_pre_request_scripts.png)

### 🧠 Observaciones técnicas
- Los scripts previos permiten modificar variables, headers, tokens, etc. antes de ejecutar la petición.
- Muy útil para generación de datos aleatorios, timestamps, tokens JWT, etc.
- Se ejecutan antes que la construcción final del request.
