# SaneCrafting-drake

[![Rama](https://img.shields.io/badge/branch-1.21--latin-2ea44f)](https://github.com/DrakesCraft-Labs/SaneCrafting-drake/tree/1.21-latin)
[![Licencia](https://img.shields.io/github/license/DrakesCraft-Labs/SaneCrafting-drake)](https://github.com/DrakesCraft-Labs/SaneCrafting-drake/blob/1.21-latin/LICENSE)
[![Ultimo commit](https://img.shields.io/github/last-commit/DrakesCraft-Labs/SaneCrafting-drake/1.21-latin)](https://github.com/DrakesCraft-Labs/SaneCrafting-drake/commits/1.21-latin)

## Descripción técnica
Addon que adapta recipes/research/lore para una experiencia de crafteo más limpia en Slimefun.

## Qué añade a Slimefun
- Hace más predecible y legible la progresión de crafteo.
- Reduce errores operativos en recipe discovery.
- Mejora consistencia entre research y recetas reales.

## Características principales
- Parches de recipe book y research unlock.
- Conversión/normalización de recetas para mejor UX.
- Mitigación de ruido por recetas inexistentes legacy.

## Matriz de compatibilidad
| Componente | Estado |
|---|---|
| Minecraft | 1.21.x |
| Paper/Purpur | 1.21.x |
| Slimefun Core Drake | 11.x (línea `1.21-latin`) |
| Java | 21 |

## Instalación
1. Descarga el `.jar` de Releases del repositorio.
2. Copia el archivo en la carpeta `plugins/` del servidor.
3. Asegura dependencias (`Slimefun`, `ProtocolLib` u otras según addon).
4. Reinicia el servidor y revisa `logs/latest.log` para validar carga.

## Build local
```bash
mvn -DskipTests clean package
```

Artefacto esperado:
- `target/SaneCrafting-*.jar`

## Flujo de release
1. Crear branch de cambios (`feature/*` o `fix/*`).
2. Abrir PR hacia `1.21-latin` con plan de pruebas.
3. Al mergear, crear tag/release y publicar jar compilado.

Probar en entorno con packs de addons amplios para evitar recetas huérfanas.

## Relación con el monorepo
Este repositorio se mantiene en paralelo con `drakes-slimefun-labs` para desarrollo aislado por addon y despliegues independientes.