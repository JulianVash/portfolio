🌿 Git y Conventional Commits en el Monorepo

## 1. ¿Por qué Conventional Commits?
En este proyecto, la gestión del historial de cambios se realiza siguiendo la especificación de **Conventional Commits**. Esto aporta las siguientes ventajas:
- **Claridad e Historial Legible:** 📊 Permite entender de un vistazo qué modifica cada commit (una nueva característica, una corrección, documentación, etc.).
- **Automatización:** ⚙️ Facilita la generación futura de registros de cambios (*changelogs*) y el versionado semántico (SemVer) automático.s

### Estructura estándar utilizada:
`type(scope): description`

- **`feat`**: 🚀 Para nuevas funcionalidades (ej. `feat(angular-app): inicializar aplicacion base`).
- **`fix`**: 🛠️ Para corrección de errores.
- **`docs`**: 📚 Para cambios exclusivamente en la documentación o notas de aprendizaje.
- **`chore`**: 🧹 Para tareas de mantenimiento, configuración o herramientas.

---

## 2. Conexión Segura con GitHub mediante SSH
Para sincronizar nuestro monorepo local con el repositorio remoto en GitHub de forma segura y sin necesidad de introducir contraseñas o tokens personales en cada operación, se optó por el protocolo **SSH (Secure Shell)** en lugar de HTTPS.

### Pasos clave aplicados:
- **Vinculación del repositorio remoto:**
  ```bash
  git remote add origin git@github.com:TU_USUARIO/portfolio.git