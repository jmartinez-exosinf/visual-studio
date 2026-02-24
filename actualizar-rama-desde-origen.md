# #️⃣ Cómo actualizar tu rama desde la rama de origen en Visual Studio 2022

Este tutorial explica paso a paso cómo traer los cambios de una rama origen (por ejemplo, `main` o `develop`) hacia tu propia rama de trabajo.

> **Objetivo:**  
> Mantener tu rama local al día con los cambios más recientes del repositorio remoto.

----------

# 🎯 **Requisitos previos**

-   Tener **Visual Studio 2022**.
-   Haber clonado un repositorio Git (GitHub).
-   Estar trabajando en una rama propia (por ejemplo `feature/mi-rama`).

----------

# 🟦 1. Cambiarte a tu rama de trabajo

1.  Abre Visual Studio.
2.  En la esquina inferior derecha o en el menú **Git**, selecciona: **Git → Manage Branches** (Administrar ramas).
3.  En la lista de ramas locales, da **doble clic** en tu rama:  
    👉 `feature/mi-rama`

Esto garantizará que cualquier actualización llegue a tu rama actual.

----------

# 🟦 2. Obtener los últimos cambios del repositorio remoto (Fetch)

1.  Ve al menú superior:  
    **Git → Fetch**
2.  Ve al menú superior:  
    **Git → Pull**
3.  Visual Studio descargará los cambios nuevos del servidor, pero **sin mezclarlos todavía**.

Debes ver un mensaje tipo:  
_“Fetched origin with X updates”_.

----------

# 🟦 3. Actualizar tu rama local a partir de la rama origen

Ahora vas a mezclar los cambios más recientes de la rama origen (ej: `origin/main`) con tu rama actual.

## 🔵 A) Hacer un **Merge** (forma sencilla y segura)

1.  Abre **Git → Manage Branches**
2.  Busca la rama origen remota, por ejemplo:  
    👉 `origin/main`
3.  Clic derecho → **Merge into Current Branch**  
    (Fusionar en la rama actual)

Visual Studio aplicará los cambios directamente en tu rama.

### ✔ Resultado:

Tu rama queda sincronizada con los últimos cambios de `main` y mantiene tu historial intacto.

----------

# 🟦 4. Resolver conflictos (solo si aparecen)

Si hay conflictos, Visual Studio mostrará archivos en conflicto.

Puedes resolvrlos en: **Git Changes → Conflicts**

VS ofrece tres opciones por archivo:

-   **Take Source** (tomar cambios de la rama origen)
-   **Keep Target** (mantener tus cambios)
-   **Merge** (mezclarlos en un editor visual)

Cuando termines: Clic en **Accept Merge → Commit**.

----------

# 🟦 5. Confirmar que tu rama está actualizada

En **Git → View History** puedes verificar:

-   Commits de `main` ahora están antes de tus commits.
-   Tu rama está alineada con el resto del equipo.

----------

# 🎉 ¡Listo!

Tu rama ya está actualizada con la rama principal usando la opción exacta que mencionaste.

----------

# 📌 Consejos adicionales

### ✔ ¿Cada cuánto debo actualizar mi rama?

Idealmente **cada día**, o antes de abrir un Pull Request.
