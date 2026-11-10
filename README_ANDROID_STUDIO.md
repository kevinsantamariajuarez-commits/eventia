# EVENTIA — Proyecto Android Studio
## Del boleto digital a la experiencia inteligente
**Grupo Tecnológico Universitario Campus Toluca**
**Ingeniería y Tecnología | Septiembre 2026 — Diciembre 2026**

---

### 📱 Cómo abrir y continuar editando en Android Studio:

1. **Descomprimir el archivo ZIP**:
   Extrae esta carpeta `eventia-android` en una ruta sin espacios ni caracteres especiales (por ejemplo: `C:\Proyectos\eventia-android` o `~/AndroidStudioProjects/eventia-android`).

2. **Abrir en Android Studio**:
   - Abre Android Studio (versión Hedgehog, Iguana, Jellyfish o posterior).
   - Selecciona **"Open"** (o `File > Open`).
   - Navega y selecciona la carpeta raíz del proyecto (**eventia-android**).
   - Haz clic en **OK**.

3. **Sincronización de Gradle**:
   - Android Studio descargará automáticamente las dependencias de Gradle (Kotlin, AndroidX, Material Design 3, WebKit).
   - Asegúrate de tener configurado **JDK 17** en `File > Settings > Build, Execution, Deployment > Build Tools > Gradle > Gradle JDK`.

4. **Probar en Emulador o Celular Físico**:
   - Selecciona un emulador con Android 9.0 o superior (API 28+).
   - O conecta tu teléfono Android con la depuración USB activada.
   - Presiona el botón verde **"Run" (Shift + F10)**.

5. **Generar el archivo APK instalable**:
   - En el menú superior: `Build > Build Bundle(s) / APK(s) > Build APK(s)`.
   - Una vez finalizado, Android Studio te mostrará un aviso: *"APK(s) generated successfully"*. Haz clic en **"locate"** para copiar el archivo `app-debug.apk` a tu teléfono.

---

### 📂 Estructura de archivos del proyecto:

- `app/src/main/AndroidManifest.xml`: Declaración de permisos (Internet, Cámara para escaneo QR, Vibración).
- `app/src/main/java/com/gtu/eventia/MainActivity.kt`: Actividad principal Android con WebView optimizado, puente con JavaScript, soporte de cámara y navegación nativa con botón atrás.
- `app/src/main/java/com/gtu/eventia/WebAppInterface.kt`: Puente nativo para llamadas desde JavaScript.
- `app/src/main/res/layout/activity_main.xml`: Vista con Swipe-to-Refresh y barra de progreso.
- `app/src/main/res/values/`: Textos, colores del tema oscuro de EVENTIA y estilos.
