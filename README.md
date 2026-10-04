# OTTOCABELLOM — Simulador Hipotecario Android

Proyecto Android nativo basado en el simulador HTML proporcionado por el usuario.

## Incluye
- Sistema francés (cuota fija).
- Sistema alemán (capital fijo).
- Conversión de EAP a tasa mensual efectiva.
- Escenario 1: abonos para reducir cuota manteniendo el plazo.
- Escenario 2: abonos para reducir plazo manteniendo la cuota original.
- Abono recurrente anual.
- Abonos individuales editables por año.
- Tabla de amortización.
- Cálculos locales, sin depender de Tailwind, Chart.js ni CDN.

## Generar el APK desde el navegador

Este proyecto incluye `.github/workflows/build-apk.yml`. GitHub Actions prepara Java, Android SDK y Gradle automáticamente y genera el APK como artefacto.

1. Crea un repositorio nuevo en GitHub.
2. Sube el contenido de esta carpeta al repositorio (la carpeta `app` debe quedar en la raíz del repositorio, junto a `build.gradle` y `settings.gradle`).
3. Abre la pestaña **Actions**.
4. Selecciona **Build OTTOCABELLOM APK**.
5. Pulsa **Run workflow**.
6. Cuando termine correctamente, abre la ejecución y descarga el artefacto **OTTOCABELLOM-debug-apk**.
7. Dentro del ZIP descargado encontrarás `app-debug.apk`.

GitHub Actions es el camino recomendado para este proyecto porque no requiere Android Studio en tu PC. El workflow usa AGP 8.7.3 con Gradle 8.9, una combinación compatible según la documentación oficial de Android.

## Compilación local

Si posteriormente instalas herramientas Android, el proyecto puede abrirse en Android Studio o compilarse con Gradle.
