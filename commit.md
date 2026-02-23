# #️⃣  Cómo hacer un _commit_ en Visual Studio 2022

Un **commit** es un guardado de tus cambios en el repositorio local, con un mensaje que describe lo que hiciste.

----------

# 🟦 1. Asegúrate de que tienes cambios pendientes

En el panel **Git Changes** (normalmente a la derecha o abajo) verás:

-   Archivos modificados
-   Archivos nuevos
-   Archivos eliminados
-   Archivos renombrados

Si no ves el panel, ábrelo:

> **View → Git Changes**

----------

# 🟦 2. Seleccionar los archivos a incluir en el commit

En **Git Changes**, verás dos secciones:

-   **Changes** → Archivos sin preparar (_unstaged_)
-   **Staged Changes** → Archivos preparados para el commit

### Para preparar los archivos:

-   Clic en el símbolo **+** junto a cada archivo  
    ó
-   Clic en **Stage All** para incluir todos

Esto es lo que Git llama _"agregar al staging"_.

----------

# 🟦 3. Escribir el mensaje del commit

En la parte superior del panel **Git Changes** verás una caja de texto:

### **Message**

Aquí debes escribir un mensaje claro como:

> “Corrijo bug de login al validar tokens nulos”  
> “Agrego soporte para configuración TLS en el proxy”  
> “Actualizo estilo del formulario de usuarios”

----------

# 🟦 4. Hacer el commit

Cuando el mensaje esté listo:

🔵 Clic en **Commit**  
(Esto crea el commit _localmente_)

o si quieres hacer el commit y enviar inmediatamente al servidor:

🟣 **Commit All and Push**

----------

# 🟦 5. (Opcional) Hacer Push al repositorio remoto

Si usaste solo **Commit**, tus cambios aún están en tu computadora.

Para enviarlos a GitHub:

> **Git → Push**

Visual Studio te mostrará un mensaje de confirmación cuando se haya enviado correctamente.

----------

# 🎉 ¡Commit completado!

Tu trabajo ya quedó registrado en el historial del repositorio.
