# Bancolombia App

![version](https://img.shields.io/badge/version-1.0.0-FFD43B)
![plataforma](https://img.shields.io/badge/android-8%2B-3ddc84)
![licencia](https://img.shields.io/badge/licencia-MIT-blue)

Réplica funcional de la app Bancolombia hecha en HTML, CSS y JS puro, empaquetada con Capacitor. Tiene inicio de sesión, registro completo, clave dinámica, cuentas, movimientos, transferencias, bolsillos, facturas y trámites, todo guardado en el dispositivo.

**[Descargar APK](../../releases/latest/download/bancolombia.apk)** · **[Ver página de descarga](../../site/)**

## Cuenta de prueba

    usuario: alejandra
    clave: 123456

## Compilar el APK sin Android Studio

1. Ve a la pestaña **Actions** del repositorio.
2. Elige **Compilar APK** y pulsa **Run workflow**.
3. Al terminar, descarga el APK desde **Artifacts**.

Si publicas un tag, el APK se adjunta solo al Release:

    git tag v1.0.0
    git push origin v1.0.0

## Compilar en local

    npm install
    npx cap add android
    npx cap sync android
    cd android && ./gradlew assembleDebug

El APK queda en android/app/build/outputs/apk/debug/app-debug.apk

## Estructura

    app/                  aplicación web (index, manifest, ícono)
    site/                 página pública de descarga
    .github/workflows/    compilación del APK y publicación de la página
    capacitor.config.json configuración del contenedor Android

## Aviso

Proyecto educativo. No está afiliado a Bancolombia y no se conecta a sus servidores reales: los saldos y movimientos son simulados.

## Licencia

MIT