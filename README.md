# 📊 Power Apps – Gestión de Pagos (Canvas App)

## 🧠 Descripción

Aplicación desarrollada en **Power Apps (Canvas App)** para la gestión de registros de pagos.
Incluye funcionalidades tipo **CRUD** (crear, visualizar, editar y eliminar) utilizando colecciones locales.

Este proyecto fue construido como ejercicio práctico enfocado en:

* Manejo de datos en memoria (`Collections`)
* Diseño de interfaz (UI/UX)
* Implementación de popups modales
* Simulación de flujo real de negocio

---

## 🚀 Funcionalidades principales

### 📋 Visualización de datos

* Tabla de pagos con:

  * Fecha
  * Concepto
  * Importe
  * Forma de pago
  * Estatus

---

### ✏️ Edición de registros

* Popup modal para editar:

  * Concepto
  * Importe
  * Forma de pago
  * Estatus
* Actualización dinámica mediante `Patch()`

---

### 🗑️ Eliminación de registros

* Confirmación mediante popup
* Eliminación con `Remove()`
* Actualización inmediata de la galería

---

### 🎨 Interfaz de usuario

* Diseño basado en:

  * Contenedores responsivos
  * Galerías como tablas
  * Popups con overlay
* Indicadores visuales por estatus:

  * 🟢 Aprobado
  * 🟡 Pendiente
  * 🔴 Rechazado

---

## 🧱 Estructura del proyecto

```plaintext
/src
  ├── CanvasManifest.json
  ├── Controls/
  ├── Screens/
  ├── DataSources/
  └── ...
AplicacionPrueba3.msapp
```

---

## ⚙️ Tecnologías utilizadas

* Microsoft Power Apps (Canvas Apps)
* Power Fx (lenguaje de fórmulas)
* Power Platform CLI (`pac`)

---

## 🛠️ Cómo ejecutar el proyecto

### 🔹 Opción 1 — Power Apps (recomendada)

1. Ir a https://make.powerapps.com
2. Seleccionar **Aplicaciones**
3. Importar el archivo:

```plaintext
AplicacionPrueba3.msapp
```

4. Abrir en modo edición o ejecución

---

### 🔹 Opción 2 — Desde código (CLI)

Convertir `.msapp` a código:

```bash
pac canvas unpack --msapp "AplicacionPrueba3.msapp" --sources "./src"
```

---

## 📌 Notas técnicas

* Los datos se manejan mediante **colecciones locales (`ClearCollect`)**
* No hay conexión a backend (simulación local)
* El estado se controla mediante variables (`Set`)
* La UI se construye con galerías y contenedores

---

## 🧠 Aprendizajes clave

* Manejo de estado en Power Apps
* Uso de `Patch()` para actualización de registros
* Implementación de modales reutilizables
* Separación de lógica y presentación

---

## 🚧 Posibles mejoras

* Conexión a Dataverse o SharePoint
* Validaciones más robustas
* Manejo de errores
* Autenticación de usuarios
* Persistencia de datos

---

## 👨‍💻 Autor

Proyecto desarrollado como práctica personal.

---

## 📄 Licencia

Uso libre para fines educativos y demostrativos.
