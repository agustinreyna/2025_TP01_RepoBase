# Decisiones y flujo de trabajo – TP01

## 1. Flujo de trabajo

Usé un flujo basado en **Git Flow simplificado**:

* `main`: versión estable.
* `feature/parametros_funcion`: desarrollo de la función `saludar`.
* `hotfix/fix-saludo`: corrección rápida de un error simulado.

Esto permite trabajar sin romper `main` y aplicar fixes rápido.

---

## 2. Integración del fix

* Simulé un bug en `main`, comentando la llamada a la funcion.
* Creé la rama `hotfix/fix-saludo` y descomenté la llamada a la función.
* Integré el fix a `main` con **merge**.
* Apliqué el fix a la rama feature con **cherry-pick** para tener un commit limpio y personalizado.
* **Conflicto al cherry-pick**: se resolvió manualmente en el IDE y luego continué con `git cherry-pick --continue`.

---

## 3. Calidad y trazabilidad

* Commits claros y atómicos.
* Uso de ramas dedicadas para features y hotfixes.
* Pull Request para revisión y control de cambios.
* Tag `v1.0` para marcar la versión estable.

---