# 🐛 Bug: El botón de registro no responde en dispositivos móviles

## 📝 Descripción
Al intentar registrarse desde un navegador móvil (Safari/Chrome en iOS/Android), el botón "Finalizar Registro" se queda en estado de carga infinito o no hace nada. En escritorio funciona correctamente.

## 🎥 Evidencia
<!-- 👉 AQUÍ: Arrastra tu GIF o imagen desde tu carpeta directamente aquí 👈 -->

## 🛠️ Pasos para reproducir
1. Entrar a la URL de registro desde un móvil.
2. Llenar todos los campos obligatorios.
3. Hacer clic en el botón "Finalizar Registro".
4. *Resultado esperado:* Redirección al Dashboard.
5. *Resultado actual:* Nada, o spinner infinito.

## 🖥️ Contexto Técnico
* **Entorno:** Producción.
* **Navegadores afectados:** Safari iOS 17, Chrome Android.
* **Posible archivo afectado:** `src/components/RegisterForm.js` -> Función `handleSubmit`.

> **Nota:** Ya revisé los logs del servidor y no llega ninguna petición, parece un error de frontend.
