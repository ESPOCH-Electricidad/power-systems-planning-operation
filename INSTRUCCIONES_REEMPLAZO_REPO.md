# Instrucciones para reemplazar el repositorio local

Este paquete contiene una versión completa del repositorio público.

## Reemplazo seguro

1. Hacer `pull` del repositorio actual.
2. Crear una rama: `git checkout -b mejora-modelos-casos-actividades`.
3. Eliminar del repositorio local todo excepto la carpeta `.git`.
4. Copiar el contenido de este paquete dentro de la carpeta del repositorio.
5. Ejecutar:

```bash
git status
git add .
git commit -m "Mejora modelos, casos, actividades y documentacion publicable"
git push origin mejora-modelos-casos-actividades
```

6. Abrir Pull Request hacia `main` y revisar antes de fusionar.
