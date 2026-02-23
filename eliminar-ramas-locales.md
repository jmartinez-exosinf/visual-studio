# #️⃣ Cómo eliminar ramas locales en Visual Studio 2022

En Git, las **ramas locales** son copias que existen solo en tu máquina.  
Con el tiempo, es normal acumular ramas que ya no necesitas, especialmente cuando:

-   Ya hiciste merge de esa rama
-   Ya existe una nueva versión
-   Fue eliminada en remoto
-   Era una prueba temporal

Este tutorial te explica cómo eliminarlas de forma segura.

----------

# 🟦 1. Abrir el listado de ramas en Visual Studio

1.  En el menú superior, selecciona:  
    **Git → Manage Branches**
2.  Se abrirá el panel que muestra:
    -   Ramas locales
    -   Ramas remotas
    -   Ramas actualmente activas

----------

# 🟦 2. Verifica que NO estás en la rama que deseas eliminar

Git no permite borrar la rama en la que estás parado.

Mira la barra inferior de Visual Studio o el panel de ramas para asegurarte de que NO estás en la rama que quieres borrar.

Si lo estás:

1.  Cambia a otra rama (por ejemplo `main` o `develop`)  
    haciendo doble clic en ella.

----------

# 🟦 3. Eliminar la rama local desde Visual Studio

1.  En **Local branches**, busca la rama a eliminar.
2.  Haz clic derecho sobre la rama.
3.  Selecciona:  
    **Delete** (Eliminar)

Visual Studio te pedirá confirmación.

### ✔ Si la rama ya fue fusionada o no tiene cambios pendientes

Se eliminará sin problemas.

### ⚠ Si la rama NO ha sido fusionada

VS mostrará una advertencia indicando que puedes perder cambios.

----------

# 🟦 4. (Opcional) Forzar eliminación desde Visual Studio

Si la rama tiene cambios sin fusionar, Visual Studio te ofrecerá la opción equivalente a:

-   ✔ **Delete branch** (seguro)
-   ⚠ **Delete branch (force)** (forzar)

Solo usa esta opción si **estás completamente seguro** de que no necesitas esos cambios.

----------


# 🟦 5. Buenas prácticas al eliminar ramas locales

✔ **Hazlo solo después de merge o cuando estés seguro de que ya no se usará.**  
✔ **Haz limpieza cada 1–2 semanas**, especialmente si trabajas con muchas features.  
✔ Si no estás seguro, respalda la rama antes de borrarla.

----------

# 🎉 ¡Listo!

Ya sabes cómo eliminar ramas locales de forma segura en Visual Studio 2022.
