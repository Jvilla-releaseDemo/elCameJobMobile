# ElCameJob App - Android 🚀

# Nota > Esta version se hizo en forma de appweb por convenieniencias de los frameworks usados paa hacer la app como vite y postgrSQL.
​
 Este es el proyecto de Android generado con **Capacitor** para la aplicación **ElCameJob**. Ha sido optimizado para ofrecer el mejor rendimiento y un tamaño de instalación reducido.
​
 ## 🛠 Optimizaciones Aplicadas
​
 El proyecto cuenta con varias mejoras de nivel profesional:
​
 - **Minificación y Ofuscación (R8):** Configurado en `release` para eliminar código muerto y proteger el binario.
 - **Resource Shrinking:** Eliminación automática de recursos (imágenes, layouts) no utilizados para reducir el tamaño del APK.
 - **ABI Splits:** Generación de APKs específicos por arquitectura (`arm64`, `v7a`, `x86_64`) para que los usuarios solo descarguen lo necesario para su dispositivo.
 - **Icono Personalizado:** Se ha implementado un icono de cohete espacial nativo (Vector Drawable) que sustituye al icono por defecto de Capacitor.
 - **Modernización de Gradle:** Eliminación de `flatDir` en favor de `fileTree` para una gestión de dependencias más robusta y compatible con metadatos.
​
 ## 🚀 Cómo empezar
​
 ### Requisitos previos
 - Android Studio (versión Flamingo o superior recomendada)
 - JDK 17
 - Node.js & npm
​
​
 ### Generar el APK
 Para generar una versión de depuración (Debug):
 ```bash
 cd android
 ./gradlew assembleDebug
 ```
 El archivo se generará en: `android/app/build/outputs/apk/debug/`
​
 Para generar la versión de producción optimizada:
 ```bash
 ./gradlew bundleRelease
 ```
​
 ## ⚠️ Notas de Integración (Vercel)
 El backend está desplegado en **Vercel** usando "Deployment Protection"
​
 ## 📁 Estructura del Proyecto Android
 - `app/`: Módulo principal de la aplicación.
 - `capacitor-android/`: Librería core de Capacitor.
 - `capacitor-cordova-android-plugins/`: Soporte para plugins de Cordova.
​
