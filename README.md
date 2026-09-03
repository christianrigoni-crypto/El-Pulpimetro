# El Pulpimetro

Aplicación Android para registrar horas trabajadas y calcular ingresos por quincena y mes.

## Publicar una actualización

1. En `app/build.gradle.kts`, aumentar `versionCode` y cambiar `versionName`.
2. Generar el APK en la misma computadora para conservar la firma usada por las instalaciones anteriores.
3. En GitHub, abrir **Releases**, crear una versión nueva y adjuntar el APK con el nombre `El-Pulpimetro.apk`.
4. Editar `version.json` y colocar el nuevo `versionCode`, `versionName`, enlace directo al APK y mensaje.

Ejemplo para la versión 1.1:

```json
{
  "versionCode": 2,
  "versionName": "1.1",
  "apkUrl": "https://github.com/christianrigoni-crypto/El-Pulpimetro/releases/download/v1.1/El-Pulpimetro.apk",
  "mensaje": "Mejoras y nuevas funciones."
}
```

La aplicación consulta `version.json` al abrirse y desde el botón **Actualizaciones > Buscar**. Si el número publicado es mayor que el instalado, ofrece descargar la nueva versión.
