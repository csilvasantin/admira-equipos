# Admira Equipos

Inventario de ordenadores de las sedes de Admira, organizado por ubicación.

## Sedes

### Barcelona
| Sede | Archivo |
|---|---|
| AdmiraNext | `data/equipos/admira-next.json` |
| AdmiraXtore | `data/equipos/admira-xtore.json` |
| AdmiraXperience | `data/equipos/admira-xperience.json` |
| AdmiraXpace | `data/equipos/admira-xpace.json` |
| Admira University | `data/equipos/admira-university.json` |

### Sitges
| Sede | Archivo |
|---|---|
| Admira Sitges | `data/equipos/sitges.json` |

## Estructura

```
data/
├── sedes.json                          # Registro de todas las sedes
└── equipos/
    ├── admira-next.json                # AdmiraNext (Barcelona)
    ├── admira-xtore.json               # AdmiraXtore (Barcelona)
    ├── admira-xperience.json           # AdmiraXperience (Barcelona)
    ├── admira-xpace.json               # AdmiraXpace (Barcelona)
    ├── admira-university.json          # Admira University (Barcelona)
    └── sitges.json                     # Admira Sitges
```

## Uso

Cada archivo en `data/equipos/` contiene un array de equipos con:
- Identificador de máquina
- Nombre, tipo y plataforma
- Usuario asignado y rol
- Especificaciones técnicas (cuando se conozcan)
- Notas operativas

## Relación con otros repos

- **AdmiraNext-Team**: panel de estado en tiempo real. Este repo es el inventario estático de referencia.
- **onboarding**: el welcome pack enlaza aquí para que nuevas IAs conozcan el parque de máquinas.
