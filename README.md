# Kaptura — releases públicos

Repositorio **solo para distribución** del APK de Kaptura. No contiene código fuente.

- Código privado: [kaptura](https://github.com/INGYasen/kaptura) (privado)
- La app (futuro OTA) lee `version.json` en la rama `main`

## Instalar manualmente

1. Descarga directa: [kaptura.apk](https://media.githubusercontent.com/media/INGYasen/kaptura-releases/main/kaptura.apk)
2. O abre [Releases](https://github.com/INGYasen/kaptura-releases/releases) si hay un release publicado
3. Instala en el teléfono (permite “orígenes desconocidos” si Android lo pide)

## Publicar una nueva versión (desde tu PC)

```powershell
cd "D:\app kaptura"
.\scripts\publish-release.ps1 -Version "0.10.14" -Build 24 -Changelog "Notas de la versión"
```

El script sube el APK con Git LFS y actualiza `version.json`. Si `gh auth login` está activo, también crea el GitHub Release.
