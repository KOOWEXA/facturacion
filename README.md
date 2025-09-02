# Factura Fácil 💼📄

Una aplicación web simple y autónoma para generar facturas electrónicas directamente desde el navegador. Sin servidor, sin instalación, sin datos personales expuestos.

✨ 100% cliente  
🎨 Tema claro/oscuro  
📥 Genera PDF  
📧 Enviar por Gmail  
💾 Guarda datos localmente

---

## 🔧 Características

- Generación automática de número de factura único
- Formulario con validación (campos obligatorios, CI, correo)
- Creación de PDF con formato profesional (usa `jsPDF`)
- Tema oscuro/claro con persistencia en `localStorage`
- Guardado local de clientes
- Botón para abrir Gmail con destinatario prellenado
- Favicon SVG incrustado (sin archivos externos)
- Diseño responsive y accesible
- Código limpio y modular (IIFE)

---

## 🖥️ Demo

👉 [Ver demo](https://tudominio.github.io/factura-facil) *(actualiza con tu URL después de publicar)*

> ⚠️ Nota: El navegador no permite adjuntar archivos vía `mailto`. El botón "Enviar por Gmail" abre una ventana prellenada; el usuario debe adjuntar manualmente el PDF descargado.

---

## 🚀 Cómo Usar

1. Abre `index.html` en tu navegador.
2. Rellena los datos del cliente.
3. Haz clic en **"Generar PDF"** para descargar la factura.
4. Usa **"Enviar por Gmail"** para abrir Gmail con el correo del cliente.
5. Usa **"Guardar Local"** para almacenar los datos en el navegador.
6. Usa **"Limpiar"** para reiniciar el formulario.

---

## 🎨 Tema Oscuro

Haz clic en el botón (🌕/🌑) para alternar entre temas. La preferencia se guarda automáticamente.

---

## 💾 Almacenamiento Local

Los datos del cliente se guardan en `localStorage`. Puedes verlos en la consola con:

```js
JSON.parse(localStorage.getItem("facturas")) || []
