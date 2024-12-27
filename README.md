Aquí tienes el contenido del README en formato **Markdown** listo para ser añadido al repositorio:

```markdown
# **Inlaze Test Automation**

## **Descripción del Proyecto**
Suite de pruebas automatizadas para validar las funcionalidades de registro e inicio de sesión de la plataforma **Inlaze**.  
El proyecto utiliza **Selenium**, **TestNG**, y un diseño basado en **Page Object Model (POM)**, lo que garantiza un mantenimiento sencillo y una ejecución robusta. Los reportes detallados de las ejecuciones se generan mediante **ExtentReports**, proporcionando un resumen visual de los resultados.

---

## **Características**
- **Pruebas Automatizadas**: 
  - Validación de los flujos principales de registro e inicio de sesión.
  - Capturas de pantalla automáticas en cada prueba.
- **Gestión Automática de Drivers**:
  - Configuración automatizada del WebDriver utilizando **WebDriverManager**.
- **Reportes Avanzados**:
  - Reportes HTML generados con **ExtentReports**, mostrando estadísticas y capturas de pantalla.
- **Diseño Modular**:
  - Implementación del patrón **Page Object Model (POM)** para una estructura escalable.
- **Compatible con CI/CD**:
  - Diseñado para integrarse fácilmente con herramientas como Jenkins o GitHub Actions.

---

## **Tecnologías Utilizadas**
- **Lenguaje**: Java
- **Framework de Pruebas**: TestNG
- **Automatización del Navegador**: Selenium
- **Gestión de Drivers**: WebDriverManager
- **Reportes**: ExtentReports
- **Herramienta de Construcción**: Gradle
- **IDE**: IntelliJ IDEA

---

## **Estructura del Proyecto**
```
src/
├── main/
│   └── java/
│       ├── pages/                 # Clases Page Object Model
│       └── utils/                 # Clases auxiliares (ExtentManager, WebDriverConfig, TestUtils)
├── test/
│   └── java/
│       └── tests/                 # Clases de Pruebas TestNG (LoginTests, SignUpTests)
build.gradle                       # Configuración de Gradle
testng.xml                         # Suite de pruebas TestNG
screenshots/                       # Capturas de pantalla generadas automáticamente
extent-report.html                 # Reporte HTML generado por ExtentReports
```

---

## **Requisitos Previos**
Antes de ejecutar este proyecto, asegúrate de tener instalados los siguientes requisitos:
1. **Java JDK 8 o superior**.
2. **Gradle** (opcional si usas el Wrapper de Gradle incluido).
3. **IntelliJ IDEA** u otro IDE compatible con Gradle.

---

## **Instrucciones de Configuración**
1. Clona este repositorio:
   ```bash
   git clone https://github.com/tuusuario/inlaze-test-automation.git
   ```
2. Abre el proyecto en **IntelliJ IDEA**.
3. Sincroniza las dependencias de Gradle.
4. Configura el navegador (opcional; manejado automáticamente por WebDriverManager).

---

## **Cómo Ejecutar las Pruebas**
1. Ejecuta todas las pruebas:
   ```bash
   gradle test
   ```
2. Ejecuta un conjunto de pruebas específicas definido en `testng.xml`:
   - Haz clic derecho en el archivo `testng.xml` y selecciona **Run**.
3. Visualiza los reportes:
   - Abre el archivo `extent-report.html` generado en la raíz del proyecto para ver los resultados.

---

## **Casos de Prueba Automatizados**
### **Registro de Usuario**
1. Validar el registro exitoso con datos válidos.
2. Verificar la validación del campo "Nombre Completo".
3. Validar el formato del correo electrónico.
4. Comprobar que la contraseña cumpla con los requisitos.
5. Validar que el formulario no se envíe con campos obligatorios incompletos.
6. Verificar que el sistema maneje contraseñas que no coincidan.

### **Inicio de Sesión**
1. Validar el inicio de sesión con credenciales correctas.
2. Validar mensajes de error con credenciales incorrectas.
3. Comprobar que no se envíe el formulario con campos vacíos.
4. Verificar la redirección al registro desde el formulario de inicio de sesión.

---

## **Contribuciones**
Si deseas contribuir a este proyecto:
1. Crea un fork del repositorio.
2. Realiza tus cambios en una rama:
   ```bash
   git checkout -b feature/nueva-funcionalidad
   ```
3. Realiza un pull request describiendo tus cambios.

---

## **Licencia**
Este proyecto está bajo la licencia [MIT](LICENSE).

---

¡Con esta estructura, tu proyecto estará completamente documentado en GitHub! Si necesitas ayuda para modificar o ampliar este archivo, no dudes en decirlo. 😊
```
