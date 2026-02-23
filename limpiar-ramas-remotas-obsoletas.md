# #️⃣ Cómo limpiar ramas remotas obsoletas en Visual Studio 2022

### (Habilitando “Prune remote branches during fetch”)

Cuando trabajas con GitHub desde Visual Studio 2022, es común que el listado de ramas remotas siga mostrando ramas que ya fueron eliminadas en el servidor.  

Para evitar esto, Visual Studio incluye una función llamada **“prune”** que limpia automáticamente esas referencias.

Este tutorial te guía paso a paso para activar esa función y mantener tu lista de ramas siempre actualizada.

----------

# 🟦 1. Abrir la configuración de Git en Visual Studio

1.  En Visual Studio 2022, ve al menú superior:  
    **Git → Settings**
2.  Se abrirá una ventana con varias secciones de configuración.

----------

# 🟦 2. Acceder a las configuraciones de Git

Dentro de la ventana de Settings:

1.  En el panel izquierdo, selecciona:  
    **Git → Global Settings**  
    _(O puedes seleccionar **Repository Settings** si solo quieres hacerlo para el repo actual.)_

----------

# 🟦 3. Activar la opción de “Prune”

En la sección de configuración de Git:

1.  Busca la opción:  
    **✔ Prune remote branches during fetch**  
    (En español puede aparecer como **“Podar ramas remotas durante fetch”**)
2.  Activa la casilla.

> Esto le indica a Visual Studio que cada vez que ejecutes un `Fetch`, elimine automáticamente todas las referencias a ramas remotas que ya no existen en GitHub.

----------

# 🟦 4. Ejecutar un “Fetch” para limpiar la lista

Una vez activado el prune:

1.  Ve al menú:  
    **Git → Fetch**
2.  Visual Studio descargará actualizaciones de GitHub **y limpiará las ramas remotas obsoletas**.

Puedes verificar la lista en:

> **Git → Manage Branches → Remotes → origin**

Verás que ahora solo aparecen las ramas reales que existen en el repositorio remoto.

----------

# 🟦 5. (Opcional) Refrescar manualmente la vista

A veces la UI tarde medio segundo en actualizar.

Si no ves el cambio:

-   Clic en **Refresh** dentro de _Manage Branches_
-   O cierra y abre de nuevo el panel

----------

# 🎉 ¡Listo!

A partir de ahora:

-   Tu listado de ramas remotas siempre estará limpio.
-   Cualquier rama borrada en GitHub desaparecerá automáticamente al hacer **Fetch**.
-   No tendrás ramas “fantasma” ocupando espacio visual o generando confusión.
