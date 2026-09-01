# Kaptura — releases públicos

Repositorio **solo para distribución** del APK de Kaptura. No contiene código fuente.

- Código privado: [kaptura](https://github.com/INGYasen/kaptura) (privado)
- La app (futuro OTA) lee `version.json` en la rama `main`

## Instalar manualmente

1. Abre [Releases](https://github.com/INGYasen/kaptura-releases/releases)
2. Descarga `kaptura.apk` de la última versión
3. Instala en el teléfono (permite “orígenes desconocidos” si Android lo pide)

## Publicar una nueva versión (desde tu PC)

1. Genera el APK: `D:\app kaptura\scripts\install-phone.ps1` (o copia desde `.cache\kaptura-phone-debug.apk`)
2. En GitHub → **Releases** → **Draft a new release**
3. Tag: `v0.10.13` (igual que `version` en `version.json`)
4. Sube `kaptura.apk`
5. Actualiza `version.json` en `main` con la URL del release y haz push
